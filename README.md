This is a simple test checking dnode compatiblity on the console as shown here:

https://github.com/substack/dnode/blob/master/README.markdown

I am doing each example independently so I can just pull it down and run it seperately.

git clone https://github.com/rockhowse/dnode-test-console.git

Then run the following commands to install the proper node.js dependencies (dnode and friends) for this project:

C:\Users\Sexbox\Desktop\nodejs>cd dnode-test-console
C:\Users\Sexbox\Desktop\nodejs\dnode-test-console>npm i
npm http GET https://registry.npmjs.org/dnode
npm http 200 https://registry.npmjs.org/dnode
npm http GET https://registry.npmjs.org/dnode/-/dnode-0.9.3.tgz
npm http 200 https://registry.npmjs.org/dnode/-/dnode-0.9.3.tgz
npm http GET https://registry.npmjs.org/socket.io/0.8.6
npm http GET https://registry.npmjs.org/lazy
npm http GET https://registry.npmjs.org/traverse
npm http GET https://registry.npmjs.org/dnode-protocol
npm http GET https://registry.npmjs.org/jsonify
npm http GET https://github.com/substack/socket.io-client/tarball/master
npm http 200 https://registry.npmjs.org/jsonify
npm http 200 https://registry.npmjs.org/lazy
npm http 200 https://registry.npmjs.org/traverse
npm http GET https://registry.npmjs.org/traverse/-/traverse-0.4.6.tgz
npm http 200 https://registry.npmjs.org/dnode-protocol
npm http 200 https://registry.npmjs.org/socket.io/0.8.6
npm http GET https://registry.npmjs.org/socket.io/-/socket.io-0.8.6.tgz
npm http 200 https://github.com/substack/socket.io-client/tarball/master
npm http 200 https://registry.npmjs.org/traverse/-/traverse-0.4.6.tgz
npm http 200 https://registry.npmjs.org/socket.io/-/socket.io-0.8.6.tgz
npm http GET https://registry.npmjs.org/traverse
npm http GET https://registry.npmjs.org/redis/0.6.7
npm http GET https://registry.npmjs.org/policyfile/0.0.4
npm http GET https://registry.npmjs.org/xmlhttprequest/1.2.2
npm http GET https://registry.npmjs.org/websocket-client/1.0.0
npm http GET https://registry.npmjs.org/uglify-js/1.0.6
npm http 304 https://registry.npmjs.org/traverse
npm http 200 https://registry.npmjs.org/redis/0.6.7
npm http GET https://registry.npmjs.org/redis/-/redis-0.6.7.tgz
npm http 200 https://registry.npmjs.org/policyfile/0.0.4
npm http GET https://registry.npmjs.org/policyfile/-/policyfile-0.0.4.tgz
npm http 200 https://registry.npmjs.org/xmlhttprequest/1.2.2
npm http GET https://registry.npmjs.org/xmlhttprequest/-/xmlhttprequest-1.2.2.tgz
npm http 200 https://registry.npmjs.org/websocket-client/1.0.0
npm http GET https://registry.npmjs.org/websocket-client/-/websocket-client-1.0.0.tgz
npm http 200 https://registry.npmjs.org/uglify-js/1.0.6
npm http GET https://registry.npmjs.org/uglify-js/-/uglify-js-1.0.6.tgz
npm http 200 https://registry.npmjs.org/policyfile/-/policyfile-0.0.4.tgz
npm http 200 https://registry.npmjs.org/redis/-/redis-0.6.7.tgz
npm http 200 https://registry.npmjs.org/xmlhttprequest/-/xmlhttprequest-1.2.2.tgz
npm http 200 https://registry.npmjs.org/websocket-client/-/websocket-client-1.0.0.tgz
npm http 200 https://registry.npmjs.org/uglify-js/-/uglify-js-1.0.6.tgz
dnode@0.9.3 ./node_modules/dnode
├── jsonify@0.0.0
├── lazy@1.0.7
├── traverse@0.4.6
├── dnode-protocol@0.1.1 (traverse@0.5.2)
├── socket.io@0.8.6 (policyfile@0.0.4 redis@0.6.7)
└── socket.io-client@0.8.6

At this point, you can start up the server:

C:\Users\Sexbox\Desktop\nodejs\dnode-test-console>node server.js

Open up another console and start up the client:

C:\Users\Sexbox\Desktop\nodejs\dnode-test-console>node client.js
n = 6600

tada! simple remote method run on the server using dnode =)

-rOcK



