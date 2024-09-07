# Spring Security w/ JWT Introduction (Authentication & Authorization)

This application was built as practice to become familiar with the Spring Framework and the Spring Security Project. Registration and Login implemented using In-Memory and Database users. Application security has been configured using SecurityFilterChain, UserDetailsService, AuthenticationProvider, PasswordEncoder, and more.
A JWT is generated when an existing user is authenticated and that token can be used for further authorization when accessing protected API's.

Instructions:
1. Create a JWTSecretGeneratorTest Class & Method
2. Create a JWTService Class
3. Create a Method to Generate Token from UserDetails
4. Create a Method to Generate Secret Key for Signature from Decoded Secret Byte Array
5. Create an Endpoint to Authenticate Using LoginRequest DTO
6. Authenticate LoginRequest DTO Using AuthenticationManager and Generate Token Using JWTService
7. Create a JwtAuthenticationFilter to Extract Information from Request Headers
8. Modify Security Configuration to Add the JwtAuthenticationFilter Before UsernamePasswordAuthenticationFilter
9. Create a UsernamePasswordAuthenticationToken and Set the SecurityContextHolder with That Token
