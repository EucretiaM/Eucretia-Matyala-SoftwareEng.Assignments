```mermaid
classDiagram
    class AuthController {
        +login()
        +register()
    }
    class AuthService {
        +validateCredentials()
        +generateToken()
    }
    class AuthMiddleware {
        +checkToken()
    }
    class UserController {
        +getUserProfile()
        +updateUserProfile()
    }
    class UserService {
        +getUserData()
        +updateUserData()
    }
    class UserModel {
        +_id
        +email
        +name
        +passwordHash
    }
    class AIController {
        +requestRecommendation()
        +receiveAIResponse()
    }
    class AIService {
        +callAIAPI()
        +processAIResponse()
    }
    class AIModel {
        +responseType
        +recommendationData
    }
    class MongoDBModel {
        +userSchema()
        +mathContentSchema()
        +reportSchema()
    }

    AuthController --> AuthService
    AuthService --> AuthMiddleware
    UserController --> UserService
    UserService --> UserModel
    AIController --> AIService
    AIService --> AIModel
    MongoDBModel --> UserModel
    MongoDBModel --> MathContentModel
    MongoDBModel --> ReportModel
