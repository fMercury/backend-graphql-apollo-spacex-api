# Backend-GraphQL-Apollo-Test

npm install
npm install apollo-datasource-rest --save
-------------------------------------------------

query GetLaunches {
  launches(pageSize: 3) {
    launches {
      id
      mission {
        name
      }
      rocket {
        id
        type
      }

    }
  }
}

-------------------------------------------------

query GetLaunchById($id: ID!) {
  launch(id: $id) {
    id
    rocket {
      id
      type
    }
  }
}


{ "id": 60 }