# graphql
Примеры запросов в среде GraphQL
mutation createTodo {
	createTodo(input: {text: "first_todo", userId: "1"}) {
  	user {
      id
      name
    }
    text
    done
  }
}

query findTodos {
  todos {
    text
    done
    user {
      name
    }
  }
}