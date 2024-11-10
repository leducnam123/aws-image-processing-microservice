# Image Processing Microservices on AWS

As a newly hired software engineer, your role is to develop a secure application to assist the FBI in locating missing individuals through facial recognition. This application will enable users to upload images to an FBI-managed cloud database on AWS, where facial recognition software can analyze them for potential matches.

You will be responsible for developing and deploying a Node.js server application on AWS Elastic Beanstalk. This server will provide a RESTful API endpoint that accepts incoming image URLs.
## Getting Started

You can clone this repo to run the project locally, or test through Elastic Beanstalk.

## Project Instructions

* Set up node environment

  Initialize a new project: ```npm i```

  run the development server with ```npm run start```

* Create a new endpoint in the ```server.js``` file

  In the ```server.js``` file, create a new endpoint that uses query parameters to download an image from a public URL, apply image filtering, and return the filtered image.
  
  Helper functions to handle file processing in the ```util/util.ts``` file.

* Deploying your system

  Using ```eb init``` to create a new application, ```eb create``` to create a new environment for deploying image-filter service

## Testing

http://image-processing-microservice-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://dfstudio-d420.kxcdn.com/wordpress/wp-content/uploads/2019/06/digital_camera_photo-980x653.jpg

## License

[License](LICENSE.txt)
