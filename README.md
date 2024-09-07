# Spring Security w/ JWT Introduction (Authentication & Authorization)

This application was built as practice to become familiar with the Spring Framework and the Spring Security Project. Registration and Login implemented using In-Memory and Database users. Application security has been configured using SecurityFilterChain, UserDetailsService, AuthenticationProvider, PasswordEncoder, and more.
A JWT is generated when an existing user is authenticated and that token can be used for further authorization when accessing protected API's.

Instructions:
1. Create a JWT Secret Generator Test Class & Method
2. Create a JWT Service Class
3. Create a Method to Generate Token from UserDetails
4. Create a Method to Generate Secret Key for Signature from the decoded Secret byte array
5. Create an Endpoint to Authenticate Using LoginRequest DTO (requires AuthenticationManager bean, composed of an AuthenticationProvider)
6. Authenticate LoginRequest DTO Using AutheticationManager and Generate Token Using JwtService (UsernamePasswordAuthenticationToken)
7. Create a JwtAuthenticationFilter to extract information from the Request Headers such Authorization header, JWT string, Username, and Validate Expiration date (extend OncePerRequestFilter)
8. Create a UsernamePasswordAuthenticationToken and set the SecurityContextHolder with that token
9. Configure Security to add the JwtAuthentication filter before UsernamePasswordAuthenticationFilter
