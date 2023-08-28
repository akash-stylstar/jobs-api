# jobs-api

Database Connection
Import connect.js
Invoke in start()
Setup .env in the root
Add MONGO_URI with correct value

# Routers
- auth.js
- jobs.js
- User Model
- Email Validation Regex

# Register User
- Validate - name, email, password - with Mongoose
- Hash Password (with bcryptjs)
- Save User
- Generate Token
-Send Response with Token

# Login User
- Validate - email, password - in controller
- If email or password is missing, throw BadRequestError
- Find User
- Compare Passwords
- If no user or password does not match, throw UnauthenticatedError
- If correct, generate Token
- Send Response with Token

# Mongoose Errors
- Validation Errors
- Duplicate (Email)
- Cast Error

#Security
- helmet
- cors
- xss-clean
- express-rate-limit
