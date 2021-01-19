# 03-sprint-3 Notes
# Install your augur
1. Login as your user teamname@sociallycompute.io and the password is shared in Canvas Group Announcements. 
2. Create a virtualenvs directory
3. `virtualenv --python=python3 virtualenvs/badgers-demo`
4. Activate the virtual environment `source virtualenvs/badgers-demo/bin/activate`
5. `cd github/teamname-demo`
6. `make rebuild-dev` (for the project fork directory it will be `make install-dev`, because you'll have to pass it information specific to your instance)
7. `augur config init-frontend` : This will put a frontend configuration file in the frontend directory of Augur's root. 
8. Edit `frontend/frontend.config.json` to resolve to your hostname. For example, the atoms family looks like this (See post in slack for your assigned port ranges): 
```
{
    "Frontend": {
        "host": "atoms.sociallycompute.io",
        "port": "5100"
    },
    "Server": {
        "cache_expire": "3600",
        "host": "0.0.0.0",
        "port": "5100",
        "workers": 4,
        "timeout": 60
    }
}
```
9. `cd frontend`
10. `npm run build` : This will compile the ports into the typescript and Vue framework files. 
11. You'll have by default teamname.sociallycompute.io as an nginx route to your teamname-demo directory.  Just ask me to configure one of my subdomains or yours in nginx for teamname-project clone of your fork that you are going to create. 
12. Start Augur's backend: `nohup augur backend start >logs/team.log 2>logs/team.err &`
13. Check the logs directory, make sure there not any errors.  To see if your backend is running already, you do `ps -ef | grep virtualenv-name`. For example `ps -ef | grep badgers-demo`
14. To stop Augur: `augur backend stop` (make sure you have activated your virtualenv *first*. ) ... I usually, after the stop, to be doubly sure, do an `augur backend kill` ... maybe 30 seconds. 
15. To recall prior commands, you can always type `history`, and you'll see your previous commands. 



# Ports for Each Team
## atoms
workers: 51000 - 51200
server/frontend: 5100 & 5101


## badgers
workers: 51201 - 51400
server/frontend: 5102 & 5103

## bears
workers: 51401 - 51600
server/frontend: 5104 & 5105

## dc
workers: 51601 - 51800
server/frontend: 5106 & 5107

## eagles
workers: 51801 - 52000
server/frontend: 5108 & 5109

## gg
workers: 52201 - 52400
server/frontend: 5110 & 5111

## giants
workers: 52401 - 52600
server/frontend: 5112 & 5113

## lions
workers: 52601 - 52800
server/frontend: 5114 & 5115

## packers
workers: 52801 - 53000
server/frontend: 5116 & 5117


## tigers
workers: 53001 - 53500
server/frontend: 5118 & 5119

## vikings
workers: 53601 - 53800
server/frontend: 5120 & 5121