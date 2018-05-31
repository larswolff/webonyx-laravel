# Example schema.graphql
Place this file in the config directory of your laravel installation.

	schema {
	    query: Query
	    mutation: Mutation
	}

	type Query {
	    ping: String!
	}

	type Mutation {
	    login(data:LoginInput!): LoginOutput
	}

	type User {
	    id: Int!
	    email: String!
	}

	input LoginInput {
	    email: String!
	    password: String!
	}

	type LoginOutput {
	    token: String!
	    user: User!
	}


