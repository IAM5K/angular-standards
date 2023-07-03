# Security based questions on Angular
1. What are the Best Practices?
   1. Keep current with the latest Angular library releases.
   2. Don't alter your copy of Angular.
   3. Avoid Angular APIs marked in the documentation as **"Security Risk"**
2. What is XSS or cross site scripting?\
   Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into otherwise benign and trusted websites. XSS attacks occur when an attacker uses a web application to send malicious code, generally in the form of a browser side script, to a different end user.
3. What can enable attackers to inject arbitrary code into your application.\
   Unlike values to be used for rendering, Angular templates are considered trusted by default, and should be treated as executable code. Never create templates by concatenating user input and template syntax. Doing this would enable attackers to inject arbitrary code into your application. To prevent these vulnerabilities, always use the default Ahead-Of-Time (AOT) template compiler in production deployments.
4. What is Ahead of Time compilation in angular?\
   Ans: Ahead of Time compilation in angular markdown is a process that converts Angular templates into JavaScript code that can be executed by the browser. This process is done at build time, which means that it is not necessary to wait for the browser to compile the templates when the application is loaded. This can improve the performance of Angular applications, especially for applications that use complex templates.
5. What is sanitization?\
   Sanitization is the inspection of an untrusted value, turning it into a value that's safe to insert into the DOM. In many cases, sanitization doesn't change a value at all. Sanitization depends on context: A value that's harmless in CSS is potentially dangerous in a URL.
6. To mark a value as trusted, inject DomSanitizer and call one of the following methods:
    - `bypassSecurityTrustHtml`
    - `bypassSecurityTrustScript`
    - `bypassSecurityTrustStyle`
    - `bypassSecurityTrustUrl`
    - `bypassSecurityTrustResourceUrl`
7. 
