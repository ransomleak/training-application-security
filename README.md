# Free Secure Coding & Application Security Training — Open Source SCORM Exercises

**40 free, open-source secure coding exercises** that teach web application security the way developers learn — by exploiting real vulnerabilities like SQL injection, cross-site scripting (XSS), and broken access control, then writing the fix. Interactive SCORM modules covering the OWASP Top 10 for Web, API, Git repository security and much more. Remediation examples in JavaScript, TypeScript, Java, C#, Python, Scala, PHP, Ruby, Go, and Kotlin.

![Hands-on secure coding exercise](/Assets/demo.gif)

👥 **[Talk to the Founders](https://ransomleak.com/contact-us/)**  &nbsp;|&nbsp; 🔗 **[Browse the Full Library](https://ransomleak.com/learning)** &nbsp;|&nbsp; 🎮 **[Try a live DOM XSS demo](https://ransomleak.com/exercises/dom-xss/)**


---

## Why hands-on secure coding training works better than slides

Reading the OWASP Top 10 once a year and passing a multiple-choice quiz does not prevent web application vulnerabilities in production. Developers need to see what a real exploit does — SQL injection dumping a database, cross-site scripting hijacking a session, broken access control exposing another user's data — and then write the secure code that stops it.

**Every exercise in this library follows a three-phase methodology: exploit, trace, remediate.**

You run a hands-on penetration test against an intentionally vulnerable application — SQL injection against a database, XSS that fires in a browser, SSRF that reaches the cloud metadata endpoint — then trace exactly how the vulnerability was introduced and apply secure coding best practices to fix it.

Exercises cover:

- **OWASP Top 10 web application vulnerabilities** — broken access control, injection (SQL injection, command injection), cross-site scripting (DOM XSS, reflected XSS, stored XSS), CSRF, SSRF, directory traversal, security misconfiguration, session fixation, and more.
- **OWASP API Security Top 10** — broken object-level authorization (BOLA), broken function-level authorization, broken authentication, mass assignment, excessive data exposure, security misconfiguration, insufficient logging and monitoring.
- **Git & supply chain security** — leaked secrets in commit history, exposed .git directories, CI/CD pipeline attacks, malicious pull requests, branch protection bypass, access token leakage.
And more!

Every exercise ends with a quiz at a 100% pass threshold. By the time a developer is writing production code, they have already exploited every common web application vulnerability and know the secure coding best practices that prevent it.

---

## SCORM secure coding packages — ready for your LMS

Every exercise ships as a **SCORM 1.2 .zip** — import into any LMS (Moodle, SAP SuccessFactors, Cornerstone, TalentLMS, or anything SCORM-compliant), embed into your SDLC training pipeline, or preview on [SCORM Cloud](https://cloud.scorm.com/) before rollout.

**White-labeled** — no logos, no backlinks, no vendor lock-in. Use them as part of a DevSecOps program, a secure SDLC initiative, or standalone application security training.

---

## License

[![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

Licensed under [Creative Commons Attribution-NonCommercial 4.0 International][cc-by-nc]. You may use, adapt, and redistribute with attribution for any non-commercial purpose — internal training, workshops, university courses. Reselling the content as a standalone product is not permitted.

---

## Enterprise application security training

### For engineering & DevSecOps teams

Need secure coding training at scale without running your own LMS? We ship an **[enterprise cloud platform](https://ransomleak.com/features/)** purpose-built for application security training across engineering teams. **[Get in touch](https://ransomleak.com/contact-us/)** to see it in action.

- **Role-based enrollment** — auto-assign exercises by team, tech stack, or risk level; build custom learning paths that map to your SDLC milestones
- **Compliance dashboards** — audit-ready completion reports for SOC 2, ISO 27001, PCI DSS, HIPAA, and NIS2; export to PDF, CSV, or schedule recurring deliveries
- **SSO & provisioning** — SAML 2.0, OAuth 2.0, OIDC with Okta, Azure AD, or Google Workspace; SCIM auto-provisioning so headcount changes sync automatically
- **SIEM & workflow hooks** — push completion and risk events to Splunk, Sentinel, or QRadar; Slack and Teams notifications on training milestones; full API with webhooks for custom integrations
- **Bring your own content** — upload internal secure coding guidelines, architecture decision records, or post-mortem walkthroughs alongside the exercise library

### For MSPs & consultancies

Multi-tenant from the ground up — deliver application security training across your entire client portfolio from a single pane:

- **Per-client tenants** — isolated environments with per-tenant license management, client branding, and consolidated cross-portfolio reporting
- **White-label distribution** — your domain, your logo, your client's identity; deliver via hosted tenants or per-client SCORM exports
- **Compliance evidence** — per-developer completion records for CIS Controls, CMMC 2.0, SOC 2, and the documentation cyber-insurance carriers request at renewal

Interested? **[Reach out to us](https://ransomleak.com/contact-us/)**

---

## Table of Contents

### OWASP Top 10 for Web Applications

1. [**Clickjacking**](https://ransomleak.com/exercises/clickjacking/) — Steal a click on a bank approval button by overlaying a transparent iframe, capturing a real approval, and shipping CSP frame-ancestors.

2. [**Command Injection**](https://ransomleak.com/exercises/command-injection/) — Chain a second command onto a server-side tool by tampering a captured request, watching server secrets leak, and shipping argument-list execution.

3. [**Components with Known Vulnerabilities**](https://ransomleak.com/exercises/components-with-known-vulnerabilities/) — Get code execution through an outdated library by exploiting a published CVE, running commands via a crafted upload, and bumping the version and scanning in CI.

4. [**Cross-Site Request Forgery**](https://ransomleak.com/exercises/csrf/) — Move money from a page the victim never trusted by auto-posting a cross-site transfer, seeing why cookies ride along, and adding per-session tokens and SameSite.

5. [**Directory Traversal**](https://ransomleak.com/exercises/directory-traversal/) — Read system files through a download link by escaping the intended folder, pulling /etc/passwd from the server, and canonicalising then verifying.

6. [**DOM XSS**](https://ransomleak.com/exercises/dom-xss/) — Trigger XSS the server never sees by hiding a payload in the URL hash, tracing an unsafe innerHTML sink, and swapping to textContent.

7. [**Forced Browsing**](https://ransomleak.com/exercises/forced-browsing/) — Pull an employee PII export from an unlinked route by reaching an internal URL anonymously, seeing why obscurity is not access control, and enforcing auth server-side.

8. [**Horizontal Privilege Escalation**](https://ransomleak.com/exercises/horizontal-privilege-escalation/) — Change one digit and read another customer by walking an IDOR from both sides, enumerating sequential record ids, and adding the missing ownership check.

9. [**Host Header Injection**](https://ransomleak.com/exercises/host-header-injection/) — Redirect a password-reset email to a lookalike domain by forging the X-Forwarded-Host header, stealing the clicked reset token, and pinning a configured base URL.

10. [**Insecure URL Redirect**](https://ransomleak.com/exercises/insecure-url-redirect/) — Hide a phishing page behind a real login by abusing the next parameter, seeing why the domain looks right, and allowing relative targets only.

11. [**Leftover Debug Code**](https://ransomleak.com/exercises/leftover-debug-code/) — Pull production secrets from a forgotten debug route by finding an env-dumping endpoint, reading JWT and database secrets, and failing closed with an allow-list.

12. [**PII in URL**](https://ransomleak.com/exercises/pii-in-url/) — Lift personal data straight out of a link by spotting identifiers in query strings, following the leak into logs and referrers, and rewriting to opaque tokens.

13. [**Reflected XSS**](https://ransomleak.com/exercises/reflected-xss/) — Craft a malicious URL that runs the moment it opens by reflecting a payload off a search page, understanding the victim-clicks-link flow, and escaping at the render boundary.

14. [**Server-Side Request Forgery**](https://ransomleak.com/exercises/server-side-request-forgery/) — Make the server fetch its own cloud credentials by abusing a link-preview feature, reaching the metadata endpoint, and validating outbound destinations.

15. [**Session Fixation**](https://ransomleak.com/exercises/session-fixation/) — Plant a session id and inherit the victim login by fixing a known id on the victim, watching login reuse it, and regenerating on every login.

16. [**SQL Injection**](https://ransomleak.com/exercises/sql-injection/) — Dump a database through one unguarded lookup form by exploiting a tautology payload, exfiltrating tables with UNION SELECT, and shipping the parameterized fix.

17. [**Stored XSS**](https://ransomleak.com/exercises/stored-xss/) — Plant a script in a comment and watch it fire by storing a payload in user content, seeing it execute for the next visitor, and escaping output at render time.

18. [**Token Exposure in URL**](https://ransomleak.com/exercises/token-exposure-in-url/) — Replay a session token harvested from a referrer log by catching a token in a redirect URL, replaying it into a live account, and moving it to an HttpOnly cookie.

19. [**User Enumeration**](https://ransomleak.com/exercises/user-enumeration/) — Harvest a verified customer list from a login form by reading differing error bodies, measuring response-time leaks, and unifying errors and timing.

20. [**Vertical Privilege Escalation**](https://ransomleak.com/exercises/vertical-privilege-escalation/) — Forge a role claim and become an administrator by tampering the session token, jumping from viewer to admin, and verifying tokens before trusting them.

21. [**Weak Randomness**](https://ransomleak.com/exercises/weak-randomness/) — Predict a password-reset token and take the account by sampling tokens from the generator, recovering Math.random() state, and moving to crypto.randomBytes.

22. [**XXE Injection**](https://ransomleak.com/exercises/xxe/) — Read the password file through an XML upload by submitting a crafted purchase order, resolving an external entity, and disabling entity resolution.

---

### OWASP Top 10 for API Security

1. [**Broken Function Level Authorization**](https://ransomleak.com/exercises/broken-function-level-authorization/) — Call staff-only endpoints from a read-only account by reaching admin routes as an analyst, pulling a roster and queuing a payout, and adding a router-level role guard.

2. [**Broken Object Level Authorization**](https://ransomleak.com/exercises/broken-object-level-authorization/) — Swap an id and read another rider by changing the object id in a request, harvesting records by walking ids, and enforcing per-object ownership.

3. [**Broken User Authentication**](https://ransomleak.com/exercises/broken-user-authentication/) — Brute-force a six-digit login code by attacking an unlimited verify endpoint, taking over with only an email, and rate-limiting per account with 429.

4. [**Excessive Data Exposure**](https://ransomleak.com/exercises/excessive-data-exposure/) — Read the fields the UI never shows by comparing rendered page to raw JSON, finding phone, birth date, and coordinates, and serializing a field allow-list.

5. [**Improper Inventory Management**](https://ransomleak.com/exercises/improper-inventory-management/) — Read records through a retired API version by swapping v2 for a deprecated v1, bypassing controls the new version enforces, and retiring old versions with 410 Gone.

6. [**Injection**](https://ransomleak.com/exercises/injection/) — Turn a search box into a full database read by breaking out of a catalog query, UNION-dumping the users table, and parameterizing so input stays data.

7. [**Insufficient Logging & Monitoring**](https://ransomleak.com/exercises/insufficient-logging-and-monitoring/) — Look up a customer and leave no trace by accessing a record with no ticket, seeing why no one can attribute it, and adding audit records and alerts.

8. [**Mass Assignment**](https://ransomleak.com/exercises/mass-assignment/) — Mint a loyalty balance with two extra keys by adding fields to a PATCH body, writing attributes you should not own, and binding only editable fields.

9. [**Security Misconfiguration**](https://ransomleak.com/exercises/security-misconfiguration/) — Read a signed-in account from any website by reflecting an arbitrary CORS origin, weaponizing a lure page, and locking CORS to an allow-list.

10. [**Unrestricted Resource Consumption**](https://ransomleak.com/exercises/unrestricted-resource-consumption/) — Scrape a catalog with one oversized request by setting page size from the request, pulling 250,000 records at once, and capping page size server-side.

---

### Git & Repository Security

1. [**Secrets in Git History**](https://ransomleak.com/exercises/secrets-in-git-history/) — Recover a live API key from the commit that removed it by walking the history of a cleaned-up config file, replaying a key that was never rotated, and rotating first then scrubbing with git filter-repo.

2. [**Exposed .git Directory**](https://ransomleak.com/exercises/exposed-git-directory/) — Rebuild an entire codebase from one public URL by finding a browsable .git in the web root, dumping the repository and recovering the source, and deploying build artifacts instead of the repo.

3. [**Committed Secret Files**](https://ransomleak.com/exercises/committed-secret-files/) — Clone a public repo and read its committed .env by spotting secret files tracked since the first commit, untracking them with git rm --cached and rotating, and adding a .gitignore plus a pre-commit hook.

4. [**Commit Author Spoofing**](https://ransomleak.com/exercises/commit-author-spoofing/) — Land a backdoor wearing a maintainer's name by harvesting an author identity from git log, reading the Unverified signature badge, and requiring signed commits for all contributors including administrators.

5. [**Branch Protection Bypass**](https://ransomleak.com/exercises/branch-protection-bypass/) — Force-push over main and skip review and CI by rewriting history on an unprotected branch, shipping unreviewed code straight to production, and requiring pull requests, reviewers, and checks.

6. [**Leaked Access Tokens**](https://ransomleak.com/exercises/leaked-access-tokens/) — Clone private repos with a token from a public gist by checking what an over-scoped token can reach, revoking and rotating instead of just deleting the gist, and reissuing fine-grained and short-lived tokens.

7. [**Malicious Pull Requests**](https://ransomleak.com/exercises/malicious-pull-requests/) — Catch a backdoor hidden inside a friendly test fix by reading the full diff instead of the description, flagging out-of-scope edits to deploy scripts, and hardening review with CODEOWNERS and fork limits.

8. [**CI/CD Secret Exposure**](https://ransomleak.com/exercises/cicd-secret-exposure/) — Lift a deploy key straight out of a public build log by finding the workflow step that echoes a secret, stopping untrusted input from running as shell commands, and pinning actions by commit SHA and rotating the key.



**Topics:** secure coding training · application security training · OWASP top 10 2025 · OWASP top 10 training · web application security · web application vulnerabilities · API security · API security training · SQL injection prevention · cross-site scripting XSS · broken access control · security misconfiguration · CSRF prevention · SSRF · secure coding exercises · secure coding best practices · DevSecOps training · application security best practices · penetration testing exercises · vulnerability training for developers · git security · CI/CD security · supply chain security · SCORM security training · free application security training · open source secure coding · developer security training · shift-left security · hands-on security training · interactive security training · OWASP training for developers
