# Alexeeva Ksenia
## Contacts:
**E-mail**: ksenia1.98@mail.ru

**Telegram**: [@KsAlexa](https://t.me/KsAlexa)

**GitHub**: [KoshaScosha](https://github.com/KoshaScosha)

**LinkedIn**: [Ksenia Alexeeva](https://www.linkedin.com/in/ksenia-alexeeva-203929233/)
## About me:
I became interested in the field of IT, started self-study, now after studying the theory and basic tools for work, I want to gain practical experience on projects and improve my skills. Even if I don’t have much experience, I will try to do my best to quickly enter the process and remove some part of the load from the higher grades.
## Skills:
- Understanding of client-server architecture
- Knowledge of testing theory (SDLS, STLS, test design techniques, types of testing, test documentation, software development methodologies)
- API fundamentals: REST and SOAP
- Basic knowledge of Python (loops, functions, dictionaries, lists, debugging code through breakpoints, it’s difficult with OOP, but I’ll finish it :))
- Git/GitHub
- Basic knowledge of SQL (can use selects and joins)
- Postman
- Swagger
- I can distinguish JSON from XML, understand HTML, CSS
- Familiar with testing tools: Chrome Dev Tools, Jira (ready to master any bug tracking system), Confluence, MySQL, PostgreSQL, SoapUI, Fork
## Code example:

~~~python
from typing import List

import uvicorn
from fastapi import FastAPI, Query

app = FastAPI()

myfile = open("users.txt", "a+")


@app.get("/items/{item_id}/{item_id2}")
async def read_item(item_id: int, item_id2):
    return {"item_id": item_id,
            "item_id2": item_id2}


@app.post("/users/")
async def add_users(users: List[str]):
    for user in users[:-1]:
        myfile.write(user + "\n")
    myfile.write(users[-1])
    myfile.flush()


@app.get("/user/{index}")
async def get_user(index: int):
    myfile.seek(0)
    listusers = myfile.readlines()
    return listusers[index].strip()


uvicorn.run(app, host="0.0.0.0", port=5000)
~~~

## Work experience:
### Tester
in [Ganime.io](https://ganime.io/)

from November 2021 to March 2022

Worked as a tester on a personal project of friends
- Testing the main functionality of the site
- Testing leaderboard, beauty-contest
- Testing the bot in discord
- Testing purchases through a crypto wallet

### Team Lead
in [IntSec](https://www.int-sec.ru/)

from January 2020 until now

- Planning and creating tasks for the team
- Processing of arrays of customer information related to information intellectual security
- Monitoring the results of the automatic recognition system
- Analysis and correction of graphical and numerical data arrays
- Formation of a report on the results of work
- Participation in the development of guides for new employees
- Assistance in optimizing current processes
- Collection and analysis of organizational and technical feedback

## Education and courses:
### [Peter the Great St.Petersburg Polytechnic University](https://www.spbstu.ru/)
from September 2017 to June 2021

Unfinished higher education (bachelor)

Control in technical systems, Systems and technical means of automation and control

### [RS School](https://rs.school/)
from June 2022 to August 2022

JS / FRONT-END. STAGE 0

## Language:
English level - B1