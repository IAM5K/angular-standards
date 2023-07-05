# Questions Only
## Trusted Types in Angular Applications
1. What is the purpose of Trusted Types in Angular applications?
2. How can Trusted Types help prevent cross-site scripting (XSS) attacks?
3. What is the browser support status for Trusted Types?

## Enforcing Trusted Types
4. What are the different Angular policies that can be used to enforce Trusted Types?
5. How can you configure HTTP headers for Trusted Types in your Angular application?
6. Where should you configure the HTTP headers for Trusted Types in production serving infrastructure?
7. How can you configure HTTP headers for Trusted Types during local development and end-to-end testing using Angular CLI?
8. How can you configure HTTP headers for Trusted Types during unit testing using Karma?

## Content-Security-Policy Examples
9. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular?
10. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications that use methods in DomSanitizer that bypass security?
11. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications using JIT (Just-In-Time) compilation?
12. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications that use lazy loading of modules?

## Benefits and Usage of Trusted Types
13. Why is it important to configure Trusted Types in your Angular application's web server?
14. What is the purpose of the "angular## unsafe-bypass" policy in Trusted Types?
15. When should the "angular## unsafe-jit" policy be enabled for Trusted Types?
16. How does the "angular## bundler" policy in Trusted Types relate to lazy loading of modules?
17. What is the significance of the "require-trusted-types-for 'script'" directive in the Content-Security-Policy header?
18. How does using Trusted Types simplify the auditing of application code?

## AOT Template Compiler and Template Injection
19. How does the AOT template compiler in Angular help prevent template injection vulnerabilities?
20. Why is dynamically generating and compiling templates with user data considered a security anti-pattern?

## Server-Side XSS Protection
21. How does Angular's DomSanitizer help mitigate server-side XSS vulnerabilities?
22. What is the default compiler used by Angular CLI applications, and why is it recommended for production deployments?
23. How does the AOT (Ahead-of-Time) template compiler prevent template injection vulnerabilities and improve application performance?
24. Why is it important to use a templating language that automatically escapes values to prevent XSS vulnerabilities on the server side?
25. What are the risks associated with creating Angular templates on the server side using a templating language?
26. How does Angular's DomSanitizer help protect against XSS attacks?

## Trusted Types Overview
27. Can you explain the concept of Trusted Types and their role in preventing XSS attacks?
28. How does Angular handle server-side XSS protection in the context of template injection?
29. What is the purpose of the "angular" policy in Trusted Types, and when should it be used?
30. What are some alternatives to the AOT compiler, and why are they considered security anti-patterns?

## Additional Security Topics
31. What are the security principles that Angular applications must follow?
32. Which Angular-specific APIs should be audited in a security review?
33. What is cross-site request forgery (CSRF or XSRF)?
34. How does an attacker execute a CSRF attack?
35. How can an application prevent cross-site request forgery attacks?
36. What is the same-origin policy implemented by browsers?
37. How does Angular's HttpClient support prevention of CSRF attacks?
38. Where can you find more information on secure coding practices for Angular applications?


## Duplicates (May contain new questions)

39. What is cross-site scripting (XSS), and why is it considered a common attack on the web?
40. How does Angular's cross-site scripting security model work?
41. What is the role of the DomSanitizer in mitigating server-side XSS vulnerabilities?
42. Why is it important to use a templating language that automatically escapes values to prevent XSS vulnerabilities on the server side?
43. Explain the concept of Trusted Types and their role in preventing XSS attacks.
44. How do Content Security Policy (CSP) and Trusted Types provide an extra layer of protection against XSS attacks?
45. What are the different security contexts in Angular for sanitizing untrusted values?
46. How does Angular sanitize untrusted values for HTML, styles, and URLs?
47. Can you provide an example of how Angular automatically sanitizes interpolated content?
48. When is it necessary to mark a value as trusted using the bypassSecurityTrust... methods?
49. How does Angular's AOT (Ahead-of-Time) template compiler help prevent template injection vulnerabilities and improve application performance?
50. What are the risks associated with creating Angular templates on the server side using a templating language?
51. Explain the purpose of the "angular#unsafe-bypass" policy in Trusted Types and when it should be used.
52. When should the "angular#unsafe-jit" policy be enabled for Trusted Types, and what are the potential risks involved?
53. How does the "angular#bundler" policy in Trusted Types relate to lazy loading of modules in Angular applications?
54. What is the significance of the "require-trusted-types-for 'script'" directive in the Content-Security-Policy header?
55. How can you configure HTTP headers for Trusted Types in your Angular application during local development and end-to-end testing using Angular CLI?
56. How can you configure HTTP headers for Trusted Types in your Angular application during unit testing using Karma?
57. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular?
58. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications that use methods in DomSanitizer that bypass security?
59. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications using JIT (Just-In-Time) compilation?
60. Can you provide an example of a Content-Security-Policy header specifically configured for Trusted Types and Angular applications that use lazy loading of modules?
61. How does using Trusted Types simplify the auditing of application code in terms of security?
62. What are some alternatives to the AOT compiler in Angular, and why are they considered security anti-patterns?
63. How does Angular handle server-side XSS protection in the context of template injection?
64. What is the purpose of the "angular" policy in Trusted Types, and when should it be used?
65. How does Angular's DomSanitizer help protect against XSS attacks when handling user-generated content?
66. Explain the concept of sanitization and why it is important in preventing security vulnerabilities.
67. How does Angular's default behavior treat values by considering them untrusted, and how does it sanitize and escape them to prevent XSS attacks?
68. What are some best practices for securely interacting with the DOM in Angular applications?
