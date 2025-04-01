mutation createTodo {
  createTodo(input: {text: "first todo", userId: "1"}) {
    user {
      id
      name
    }
    text
    done
  }
}

query findTools {
  todos {
    text
    done
    user {
      name
    }
  }
}