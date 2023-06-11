# SaaS Boilerplate (Sacsify | Siasify)

Sacsify helps you build your own software while providing non-core functionality such as User authentication, Authorizations, Payments etc ready made so you can focus on building your core USP. 

## Getting started

- Sign up on the website and get an access token
- Setup and verify your domain name
- Allow access to Github repo of your project
- Configure which login options you want to provide to your users 
- Configure if you want to enable inidividual or organization signups
- Configure your stripe token to receive payments from your users
- Configure the subscription plans you want to have on your app
- You can choose from fixed monthly subscriptions, per user subscriptions or rate based subscriptions
- If you choose rate based subscriptions, you have to choose events you want to create and how much you want to charge per entity
- For rate based subscription, you will have to trigger events when the user add or removes the given entity
	```
	Auth.getUser().add(ENTITY)	
	Auth.getUser().remove(ENTITY)	
	```
- Run following command to get a boilerplate 
	```
	npx create-sacsify-app {my-app}
	```
- Enter access token created on Sacsify website
- This will generate a react application boilerplate for you 
- Boilerplate includes a react component library
- It also includes getting started pages for authentication and blank SaaS website where you can build your own business logic
- You get access to logged in user using the Auth package of Sacsify
	```
	Auth.getUser()
	```
- To create an authentication page, you can directly use 
	```JSX
	<Authentication/> 
	```
	component

- To create a payments page, you can directly use 
	```JSX
	<Payment subscription="subscription"/>
	```
	component
- To show a billing page, you can directly use 
	```
	<Billing/>
	```
	component
- To show a team page, you can directly use 
	```
	<Team/>
	```
	component, it will show user his team
- For profile page
	```
	<Profile/>
	```
- For account page 
	```
	<Account/>
	```