# Trueet - Winner of the Globo Editors Lab 2018

![alt text](http://infograficos-estaticos.s3.amazonaws.com/assets-hackathon-globo/banner.jpg)

## Team - O Globo
* Luís Guilherme Julião - Journalist, specialized in fact checking and data journalism | luis.juliao@infoglobo.com.br
* Mateus Paulino - Developer, specialized in Front-End developer and perfomance | mateus.santos@oglobo.com.br
* Vinicius Ribeiro Machado - Designer, specialized in UX/UI | vinicius.machado@infoglobo.com

## About the project
The Trueet (true + tweet) tool has basically two functions: use collaborative work, through people worried about fake news in their timelines on Twitter, to spread true information about that fact, bringing fact checking to Twitter when fake news is being disseminated, and prevent a fake news spread, alerting users that are not in contact with such misinformation.

We have built a Progressive Web App (PWA) that sends notifications about fake news when it’s increasing on social media, scan the user's timeline on Twitter and identify, based on sentences and quotes (and, in the future, keywords and artificial intelligence), publications and retweets that are disseminating this specific misinformation on user’s timeline. Then the user will be able to post a default reply provided by the tool to his friends, warning them, in a cool way, about the fake news. When the fact checkers identify fake news on the Internet and write about them, the Trueet sends a notification to PWA users with a brief message about the fake news and the link to the fact checking.

We decided to use a PWA because it is light, fast and does not require installing. The tool can be used by other teams of fact checking that wish to be partners and send notifications, rising the coverage about the fake news. We understand that, in general, many notifications can be annoying to users, so the tool will send in average three notifications per week. One person will be responsible for managing the tool, controling it and choosing in which situations the notifications would be send, according to parameters such as the number of shares on social media, the degree of harm to the victims of rumors and the topic's relevance.

## About the building process
The layout of the application was made with the Sketch design software. The tool was built using PWA (Progressive Web App), a new technology from Google that works as an application, but is lighter, faster and does not require installation or request user permissions.

The bot that scans the user's Twitter timeline was built on Node.js, allowing the same programming language to be used on both sides, the front-end and the back-end, making application maintenance and scalability easier. The bot authenticates with Twitter through the twit.js package, and queries using the Twitter development API itself.

To select publications on the user's timeline, we've created a phrase comparison algorithm that can grow and join tagging and artificial intelligence techniques (IBM Watson and TensorFlow).

Implementation, technological resume:

- Programming language: JavaScript
- Development Environment: Node.js
- App Technology: Google PWA (Progressive Web Apps).
- IBM Watson (Natural language) and TensorFlow (Text classifier) ​​are future implementations
 
## Demo
- App [click here](https://marvelapp.com/44cd58g/screen/40871628), when it load, click in preview

## Presentation
- [Click to check our presentation](https://youtu.be/TCQlNxaq-Hc)

## How to run our bot
- Get into the folder TrueetBotScan, [here](TrueetBotScan)
- Download all the files
- Inside the folder, in terminal, run the followind commands
```sh
$ npm install
```
```sh
$ node bot.js
```
- That is it! The bot is running
 
## License

Copyright 2018 Luíz Guilherme Julião, Mateus Paulino da Silva Santos, Vinicius Ribeiro Machado

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
