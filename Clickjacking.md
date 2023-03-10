`Summary:` Clickjacking is a type of vulnerability that tricks a user into clicking on something they did not intend to. This can occur when an attacker overlays an invisible or transparent layer over a legitimate webpage, causing the user to interact with a hidden element.

`Severity:` Medium

`Payload:` N/A

`Complexity:` Low

`From:` Remote / External

`Steps to Reproduce:`

1. Navigate to [https://example.com](https://example.com/).
2. Inspect the page and check for any iFrame on the page.
3. If an iFrame is found, attempt to embed the page in a malicious website or page.
4. If the page is successfully embedded, attempt to interact with the page as if it were legitimate. If the page responds to your interactions, then the clickjacking vulnerability is present.

`Proof of Concept :` **Attached in the video**

`Impact:` Clickjacking attacks can lead to a wide range of issues, including unauthorized actions being performed on the user's behalf, such as clicking on hidden ads or activating malicious links. In some cases, clickjacking attacks may allow an attacker to take over user accounts, steal sensitive information or perform other malicious actions.

`Affected IP's:` IP Address Port [https://www.example.com/](https://www.example.com/) 443

`Recommendations:` To remediate this vulnerability, the website should implement X-Frame-Options headers with the 'DENY' or 'SAMEORIGIN' values to prevent the website from being embedded in a frame or iframe. This will block clickjacking attacks. Additionally, implementing the Content Security Policy (CSP) headers with the 'frame-ancestors' directive can also mitigate clickjacking vulnerabilities.

`References:`

 [https://www.owasp.org/index.php/Clickjacking_Defense_Cheat_Sheet](https://www.owasp.org/index.php/Clickjacking_Defense_Cheat_Sheet) [https://portswigger.net/web-security/clickjacking](https://portswigger.net/web-security/clickjacking) [https://www.owasp.org/index.php/Top_10_2017-A8-Insecure_Deserialization](https://www.owasp.org/index.php/Top_10_2017-A8-Insecure_Deserialization)
