# docker-learnings

Learning docker the rocking way

### Projects within

	1. args-env-nodejs-tutorial
	2. docker-multicont-tutorial
	3. docker-nodejs-tutorial
	4. docker-noderedis-tutorial
	5. docker-react-nginx-tutorial
	6. nlp-brainjs	

### Links

	1. Natural language processing with javascript
	https://medium.com/@daffl/natural-language-processing-and-machine-learning-in-javascript-249181a3b721

	2. Movie script link 
	http://www.script-o-rama.com/snazzy/table.html
	http://www.script-o-rama.com/snazzy/table2.html
	http://www.script-o-rama.com/snazzy/table3.html
	http://www.script-o-rama.com/snazzy/table4.html


	3. Docker
	https://nodejs.org/en/docs/guides/nodejs-docker-webapp/

		a. Default buid command in docker:
		   docker build .

		b. Build command with docker to tag it:
		   docker build -t sushantsahu/docker-nodejs-tutorial .

		c. Run docker with mapped port:
		   docker run -p 3000:3000 sushantsahu/docker-nodejs-tutorial

		d. To open shell within the container:
		   docker run -it sushantsahu/docker-nodejs-tutorial sh

		e. See running docker processes:
		   docker ps

		e. To open shell within container, when app is running:
		   docker exec -it <container_id> sh  

		f. docker build -f Dockerfile.dev .

		g. Docker volumes:
		   docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app 90f474cc9ef6

		h. Run tests on react docker container (-it = std input)
		   docker run -it 0655f0d6789c npm run test

	4. Docker Compose

		// -d run in background

		a. docker-compose up
		b. docker-compose up --build
		c. docker-compose up -d
		c. docker-compose down 
		d. docker-componse ps
		
	5. Docker Network
		docker run -p 3001:3001 --net=test --name="nodejs-app1-2" sushantsahu/docker-nodejs-app-1
		
	6. Persist Database
		a. In docker compose add the following:
			volumes:
			 - ./postgres-data:/var/lib/postgresql/data
			 
	7. Docker Hub
		a. docker login (username: sushantsahu)
		b. docker push sushantsahu/[name]
	
		

### Tutorials

	1. https://www.twilio.com/blog/2017/08/working-with-environment-variables-in-node-js.html

	2. https://nodejs.org/api/cli.html#cli_r_require_module
	
	3. https://scotch.io/@Mozartted/docker-networking-how-to-connect-multiple-containers
	
	4. https://stackoverflow.com/questions/41637505/how-to-persist-data-in-a-dockerized-postgres-database-using-volumes
	
	5. https://stackoverflow.com/questions/36283908/re-using-environmental-variables-in-docker-compose-yml
	
	6. https://stackoverflow.com/questions/52302770/mongo-db-persistence-in-docker-with-volumes
	
	7. https://www.imore.com/how-edit-your-macs-hosts-file-and-why-you-would-want#how-to-reset-the-hosts-file
	
