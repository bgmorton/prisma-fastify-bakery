# Bakery App with Prisma and Fastify

A sample app for managing a bakery with [Prisma](https://www.prisma.io)
and [Fastify](https://www.fastify.io).

## Running the app

1. Build the database schema:

		npx prisma migrate dev --name init
    
2. Start Prisma Studio:

		npx prisma studio
		
3. Run the server in development mode:

		npm run dev

## Set up autoloading for the app’s components

If you’d like your development environment to automatically load all plugins from the plugins directory, check out [`fastify-autoload`](https://github.com/fastify/fastify-autoload).

## REST API endpoints that the app exposes by default

Base URL: `http://localhost:3000`

Duties: `/duty`
Products: `/products`
Ingredients: `/ingredients`
Sales: `/sales`
Employees: `/employees`
Suppliers: `/supplier`

## Examples

Products w/ ingredients:
{
    "name": "Ham & Cheese",
    "type": "Sandwich",
    "category": "Kitchen",
    "price": 1.23,
    "ingredients":[
    	{
    		"id": 6
    	},
    	{
    		"id": 3
    	},
    	{
    		"id": 8
    	}
    ]
}
