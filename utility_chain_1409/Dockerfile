FROM ethereum/client-go:latest

WORKDIR /usr/utility_node
COPY uc_1409_genesis.json .
RUN geth --datadir ./uc_node init ./uc_1409_genesis.json

ENTRYPOINT ["geth"]
CMD ["--networkid", "1409", "--datadir", "./uc_node", "--port", "30304", "--rpc", "--rpcapi", "eth,net,web3,personal", "--rpcport", "8547", "--ws", "--wsport", "8548", "--bootnodes", "enode://a4a27ee96b770d2ae801c04ac32ac494e222e0b40442b0e8400a762e5097658c47d4f66530a1459c17847215315e7dab1d99481e99cfbe9988a1bf02c2083b2e@35.173.117.179:30301,enode://08a5d0bcff92d06a8c1f7acef47d37610ffc0fb5146b693111b73656e0e2001c522971124eb8321687dcf21edd87dcf04d20276c9153ce5d045f075337c362c7@35.172.92.122:30301"]
