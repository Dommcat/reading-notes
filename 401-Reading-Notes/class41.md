# 401 Advanced Python: Class 38 Reading Notes

## Summary: This class reading is about: React 4

Explain the concept of dynamic routes in Next.js and how they differ from static routes.

- Dynamic routes in Next.js allow you to create pages with variable paths based on the requested URL at runtime.
- Dynamic routes are defined using square brackets (`[]`) in the filename or within the file itself.
- They are useful for handling data-driven routes or generating pages with different content based on parameters.
- Dynamic routes are generated at runtime, whereas static routes are pre-rendered during the build process.
- Dynamic routes enable fetching data at runtime, making it possible to provide personalized and up-to-date content.
- They allow for variable URL structures by including dynamic parameters in the path.
- Dynamic routes offer code organization benefits by consolidating similar pages into a single file.
- By combining static and dynamic routes, you can create flexible and efficient web applications.

Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

- Build your Next.js application using the `next build` command to create a production-ready version.
- Choose a deployment platform such as Vercel, Netlify, AWS Amplify, or Heroku.
- Configure your deployment by linking your code repository, setting up build commands, and configuring environment variables.
- Deploy your application by pushing your code to the remote repository or triggering a manual deployment.
- Monitor and test your deployed application to ensure all functionality works as expected.
- Configure a custom domain, if applicable, by updating DNS settings or configuring domain forwarding.
- Consider scaling and maintenance options provided by the deployment platform as your application grows.

How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.

- Next.js handles static file serving through the "public" folder located in the root directory of the project.
- Any file placed inside the "public" folder is served as a static file by Next.js.
- To reference a static file, use the `public` directory prefix in the file's URL, such as `<img src="/logo.png" alt="Logo" />`.
- Next.js optimizes static assets in the "public" folder during the build process, including compression, caching headers, and filename hashing.
- Next.js integrates with CDNs for further optimization of static file delivery.
- The default folder structure for storing static assets includes folders like "images" and "styles" within the "public" directory.
- More advanced static file handling can be achieved using Next.js server middleware or third-party packages if needed.

## Re/Sources:

ChatGPT

https://nextjs.org/learn/basics/dynamic-routes

https://nextjs.org/learn/basics/deploying-nextjs-app

https://www.youtube.com/watch?v=JWCS5IdECVI

https://nextjs.org/docs/pages/building-your-application/optimizing/static-assets


## Things I want to know more about

how to get comfortable using next.js static assets



