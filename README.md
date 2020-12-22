# Cryptocurrency

A P2P server using websockets that utilizes blockchain technology to transact a created cryptocurrency. The implementation can be seen using Postman. This is a precursor of the full-stack project I'm working on.

## Get Started
* To run test scripts, use `npm run test`.

1. Use `npm run dev` to launch the first peer.
2. Connect with a second peer in a second terminal using `HTTP_PORT=3002 P2P_PORT=5002 PEERS=ws://localhost:5001 npm run dev`
3. Add as many peers as you would like and include them as comma-separated-values in the `PEERS` variable.
4. Open Postman.
5. Make requests to the endpoints in `app.js`.

* Note: Transact requests require a recipient address which can be obtained from `/public-key`. They also require a `recipient` and `amount`.

## Technologies Used

* JavaScript
* Node
* Jest
* Express
* Websockets
* Other Packages: crypto-js, body-parser, elliptic, uuid

## User Stories

* Users can send or receive cryptocurrency.
* Users can view transactions in the pool.
* Users can mine a block and be rewarded with cryptocurrency.
* Users can view an address.
* Users can view their balance.

## Future Plans

This project will be recreated with a front-end component.