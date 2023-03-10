# CSRF (Cross-Site Request Forgery)

`Summary:` Cross-site request forgery (CSRF) is a type of attack that tricks a user into performing an action on a website without their knowledge or consent. The attacker can create a malicious request that appears to come from a trusted source, such as a user's browser, and submit it to the target website. If the user is currently logged in to the website, their session may be used to carry out the attack.

`Severity:` High

`Payload:` N/A

`Complexity:` Easy

`From:` Remote / External

`Steps to Reproduce**:`

1. Create a malicious web page that includes a hidden form or script that submits a request to the target website.
2. Trick the victim user into visiting the malicious web page while they are logged in to the target website.
3. Observe whether the request is successfully executed on the target website without the victim user's knowledge or consent.
4. Provide the details of the attack and the successful execution of the request to the website's security team

`Proof of Concept:` **Explained in the video attached**

`Impact:` An attacker can exploit this vulnerability to carry out actions on behalf of the victim user, such as changing their account information, making purchases, or performing any other actions that the user is authorized to perform. This can lead to financial losses, reputational damage, or other negative consequences for the victim.

`Affected IP's:` IP Address Port

- [https://www.example.com/](https://www.example.com/) 443

`Recommendations:` To prevent CSRF attacks, the website should implement appropriate CSRF protection measures such as using CSRF tokens, checking the Referer header, and using the SameSite attribute for cookies. Additionally, the website should educate its users on how to recognize and avoid phishing attacks, which can be used to trick users into unknowingly submitting malicious requests.

`References:`

- [https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet)
- [https://portswigger.net/web-security/csrf](https://portswigger.net/web-security/csrf)
- [https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)
