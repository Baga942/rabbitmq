1. Clone the repository to your local machine:
2. Install the dependencies using npm:
   npm install or yarn install
3. Start the RabbitMQ server (Make sure it is running before proceeding):
   rabbitmq-server
   http://localhost:15672/
   login password 
   guest guest
4. Start the worker to process the tasks:
   node consumer.js
5. Start the backend API:
   node index.js
   The backend API will be available at http://localhost:3000.
   on postman
6. Enqueue a long-running task:
   curl --location '127.0.0.1:3000/process-job' \
    --header 'Content-Type: application/json' \
    --data '{"message": "I am baga"}'
   ```
# rabbitmq
