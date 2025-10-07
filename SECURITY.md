# Security Policy

## Supported Versions

The following table lists which versions of this project currently receive security updates and patches:

| Version | Supported          |
|----------|--------------------|
| 5.1.x    | ✅ Actively supported |
| 5.0.x    | ❌ Deprecated        |
| 4.0.x    | ✅ Security fixes only |
| < 4.0    | ❌ Not supported     |

---

## Reporting a Vulnerability

If you believe you’ve found a security vulnerability in this project, please **do not open a public issue**.

Instead, report it confidentially using one of the following methods:

- **Email:** [security@yourdomain.com](mailto:security@yourdomain.com)
- **GitHub Security Advisories:** [Create a private report here](https://github.com/YOUR_ORG/YOUR_REPO/security/advisories/new)

Please include:
- A clear description of the vulnerability
- Steps to reproduce (if possible)
- The affected version(s)
- Any suggested fix or mitigation

---

## Response Process

1. You’ll receive an acknowledgment within **48 hours**.
2. We’ll investigate and provide an update within **5 business days**.
3. Once confirmed, we’ll:
   - Work on a patch and release a new version.
   - Credit the reporter (if desired).
   - Publish a security advisory once the fix is available.

---

## Disclosure Policy

We follow **responsible disclosure** practices:
- We ask reporters **not to publicly disclose** issues until a fix is released.
- We coordinate with affected users, if applicable, before publicizing the vulnerability.
- After patch release, details will be published in the GitHub Security Advisory section.

---

## Security Best Practices

For developers and users of this project:
- Always use the latest supported release.
- Avoid running outdated or modified code in production.
- Review dependencies for known vulnerabilities (using `npm audit`, `pip-audit`, or similar tools).
- Enable **Dependabot** or a similar service to stay updated on dependency risks.
