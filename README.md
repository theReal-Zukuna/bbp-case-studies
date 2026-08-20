# bbp-case-studies
none of your business, I am just tracking the reports I am reading each day and maybe some podcasts and such

https://www.youtube.com/watch?v=MXH1HqTFNm0 <br>
https://www.youtube.com/watch?v=B6QZ6wrFiE0&t=3139s (first 43 min) <br>
https://www.youtube.com/watch?v=fpW-h9uT6Uo <br>
https://hackerone.com/reports/1114347 Account takeover due to misconfiguration (--the link sent when changing the email wasnt invalidated after a subsequence change to another email--) <br>
https://hackerone.com/reports/1212374 Oauth Misconfiguration Lead To Account Takeover (--Pre-Account TakeOver--)<br>
https://hackerone.com/reports/3081691 1 Click Account Takeover via Auth Token Theft on marketing.hostinger.com <br>
https://hackerone.com/reports/1245762 Account Takeover via SMS Authentication Flow (--same session1 was handled to both attacker and victim for the same endpoint that later become valid when the victim finish authentication--)(interesting) <br>
https://www.youtube.com/watch?v=1mOEUUKLXWs <br>
https://www.youtube.com/watch?v=QEyOJ86dpz0  <br> 
https://www.youtube.com/watch?v=roNUusZow48 <br>
https://www.youtube.com/watch?v=7Rd0Z1w8sXw (removing the token value when sending the email verification request is accepted) <br>
https://www.youtube.com/watch?v=28T8Y6gJRVY (pasword reset flow lead to account take over - similar to the famous gitlab double email injection vulnerability)<br>
https://www.youtube.com/watch?v=0R3xHx7fPUM (used the same jwt token from dev server in the prod server and was accepted (audience vulnerability))<br>
https://www.youtube.com/watch?v=UiNdild6gCQ (attacker can inject victim id during account creation-->victim account should be 'created again' because it no longer work properly -->attacker register a new account with the victim email  and wait for the victim verification for the email --> he can access it with the password he set)(interesting) <br>
https://www.youtube.com/watch?v=xb4klJDM2l0 (password reset flow -> ato ,set the reset token value to null) <br>
https://www.youtube.com/watch?v=VLgB2fDEMVg (a critical Oauth vuln where the custom Oauth provider enabled unauthorized clients registrations which lead to token theft) (interesting) <br>
https://hackerone.com/reports/922456 (bypassing the requirement that accounts from resource server should be email-verified during the oauth flow (oauth provider bug )) (interesting)<br>
https://hackerone.com/reports/1148364 (a user who is just a group owner can create trusted applications (which is instance admin priviliege) which let his apps (clients) being auto-trusted during the oauth flow and granted the code to the redirect uri without user consent) <br>
https://hackerone.com/reports/685007 (password reset link not expired after email changing -> scenarios include the fact that someone can create an account for a target with temporary email that the victim should change so the account "become his account" but this vuln can be a backdoor) (boring) <br>
http://hackerone.com/reports/202781 (good) <br>
