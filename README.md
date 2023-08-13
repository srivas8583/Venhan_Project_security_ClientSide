# Venhan_Project_security_ClientSide

# Spring-security-client (server.port: 8080)
# Dependencies –
Spring web, Spring Data JPA, PostgreSQL Driver, Lombok, OAuth2 Client
# Model –
UserModel (user_data), PasswordModel ( reset_pass)
# Entity –
User, PasswordResetToken, VerificationToken
# Repository –
PasswordResetTokenRepo, UserRepo , VerificationTokenRepo
extends JpaRepository
# Event –
RegistrationComp, RegistrationCompleteListener
# Service –
Interface -> UserService
Class - > UserServiceImpl (defines all the methods of interface)
# Configuration –
➢ WebSecurityConfig (using @EnableWebSecurity)
- Standard Bean class SecurityFilterChain injected with 
http methods.
- PasswordEncoder bean injected.
➢ WebClientConfig
- WebClient and OAuth2AuthorizedClientManager bean 
# injected Controller –
RegistrationController, HelloControlle
