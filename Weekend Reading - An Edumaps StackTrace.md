# Research & Experimentation

> ... This is the list of places to refresh our previous conversations and take a deeper dive into. Can also help refresh what our focus will be on

##### Angular with Express

* [Express JS](<http://expressjs.com>) - Express JS
* [MEAN Stack](http://meanjs.org/) - The frontend at this point is a MEAN stack (with a difference) -  Microservices (M - the difference), Express (E), Angular (A), Node (N)
* [Starter MEAN Kit](https://github.com/btford/angular-express-seed) - it's 3/4 years old but just shows a quick repo of angularjs (frontend) playing within expressjs (backend)

##### Webserver Discussion - for front and/or for microservices

[Express vs KOA vs Hapi](https://www.airpair.com/node.js/posts/nodejs-framework-comparison-express-koa-hapi) - each microservice that needs a web service can use any of the three or something else completely like nginx etc.

##### Map Integration 

* [Leaflet JS](http://leafletjs.com/) - Our choice of maps for now.
* [SVG Drawing](http://dynmeth.github.io/RaphaelLayer/) - Draw SVG on a map
* [D3 Polygons & Leaflet JS](https://bost.ocks.org/mike/leaflet/) - Draw SVGs with D3 on LeafletJS

> Our map integration will house the actual map logic and code - it will not sit inside the pages app - everything and anything is just a microservice which means the map can be switched out easily for a google maps integration or bing maps etc as an example.

##### MAP Data Integration

* [Turf JS](http://turfjs.org/) - Use this for localstorage data manipulation before another microservice accepts mutatations of server data such as editing, saving and recalling. The benefit of TurfJS is that it is [isomorphic](http://nerds.airbnb.com/isomorphic-javascript-future-web-apps/) in nature which suits our use case perfectly.

> Keep this seperate from the map integration as then the geojson manipulation can be generic and mutated for any dataset. This way the maps implementation can be with leafletJS, Google Maps, bing maps, yahoo maps, here maps, direct open street maps etc etc and they will still all work just fine - It can then be user's choice in future as to the map they want to use or a particular feature might be released on google maps let's say, that we means we take a decision in future to switch out the map and it all still works

##### UI Interface

* [UI Example](https://www.lucidchart.com) - Register for a free trial and use the new beta version of their UI - I'll provide a screenshot
* [Prototyping Tools](http://www.sansfrancis.co/) - use any of the prototyping tools to draw up sketches/PDFs of the UI as discussed

##### Integrations Microservices

* [Seneca JS](http://senecajs.org/) - SenecaJS
* [Microservices architecture](http://thenewstack.io/microservices-node-js/) - Evangelising of microservices in JS
* [Microservices architecture 2](http://www.richardrodger.com/seneca-microservices-nodejs#.V5XrnpOANBc) - Another article evangelising the architecture of microservices (in JS)
* [Seneca Examples](https://hueniverse.com/2015/06/02/introducing-chairo-a-hapi-js-microservices-plugin/) - Old (some not working) examples but kind of gets you started
* [Microservices Stack Tutorial](https://hueniverse.com/2015/06/02/introducing-chairo-a-hapi-js-microservices-plugin/) - using Chairo, Hapi & Seneca

#### Technical Debt & Agile

* [Sharing and Group decision is key](https://blog.codinghorror.com/paying-down-your-technical-debt/) - Technical Debt explaination.

> We must deliver the product by a certain deadline and therefore we may need to invest in technical debt. However, we must be concious in how much technical debt we invest in so once we start coding the product entirely we need to have regular meetings (to remain [Agile](http://agilemethodology.org/)) but not neccessairly following it exclusively. It is guide and we'll use what we need from it to get the job done whjich also incuring technical debt and therefore the meetings would serve at helping us review project stage, status, everyone knows what is in/out, how it works etc and what would need to be refactored later (to clear our debt) 

#### Services & Messaging Technology

* [Thrift](https://thrift.apache.org/) - Apache
* [Protocol Buffers](https://developers.google.com/protocol-buffers/) - Google
* [MessagePack](http://msgpack.org/index.html)
* [RabbitMQ](https://www.rabbitmq.com/) - Pivitol
