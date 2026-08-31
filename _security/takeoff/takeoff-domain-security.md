---
description: 'Domain security posture for Takeoff Technologies. The registrable domain is well maintained at the DNS layer — it is DNSSEC-signed with a DS record in the parent zone and publishes both SPF and DMARC — but the web tier has decayed: the marketing host www.takeoff.com has no TLS certificate at all, and status.takeoff.com presents a certificate that does not match its hostname. Only the API gateway api.takeoff.com holds a current certificate.'
domains:
- caa: []
  caa_present: false
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:dmarc-reports@takeoff.com
  dnskey_present: true
  dnssec: true
  domain: takeoff.com
  ds: 13589 8 2 78FC2F68353D880A0302900BAC971A0C5B21300E7340E49852C8CE1A5D1A0BDA
  ds_present: true
  mx: Google Workspace (aspmx.l.google.com)
  nameservers:
  - ns-cloud-b1.googledomains.com
  - ns-cloud-b2.googledomains.com
  - ns-cloud-b3.googledomains.com
  - ns-cloud-b4.googledomains.com
  spf: true
  spf_record: v=spf1 a mx include:_spf.google.com include:mail.zendesk.com include:sendgrid.net include:stspg-customer.com ip4:168.245.1.42 ip4:149.72.173.189 ip4:149.72.195.148 include:mail.zohopayroll.in ~all
hosts:
- cert_expires: Oct 14 12:56:22 2026 GMT
  cert_issuer: C=US, O=Google Trust Services, CN=WR3
  cert_not_before: Jul 16 12:02:49 2026 GMT
  cert_subject: CN=api.takeoff.com
  host: api.takeoff.com
  hsts: false
  http_version: 2
  https: true
  note: Certificate was reissued 2026-07-16, six weeks before this probe — the API tier is actively maintained even though the company's marketing site is not.
  tls_verified: true
- detail: openssl s_client reports "no peer certificate available" and SSL alert number 80 (internal error) against 18.211.166.153; the hostname is a CNAME to proxy-ssl.webflow.com / proxy-ssl-geo-2.webflow.com, so the Webflow SSL certificate for this custom domain is no longer provisioned. HTTP on port 80 answers 301 to the same unreachable https URL, leaving no reachable web presence.
  error: tls-handshake-failed
  host: www.takeoff.com
  hsts: null
  https: false
- error: tls-handshake-failed
  host: takeoff.com
  hsts: null
  http_redirect: 'HTTP/1.1 301 -> https://www.takeoff.com/ (X-Cluster-Name: us-east-1-prod-hosting-red)'
  https: false
- detail: CNAME to qth8l8vxd7y4.stspg-customer.com (Atlassian Statuspage); the presented certificate carries no SAN for status.takeoff.com.
  error: tls-certificate-name-mismatch
  host: status.takeoff.com
  hsts: null
  https: false
kind: domain-security
layout: security
method: probed
name: Takeoff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TakeOff, probed live across 4 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TakeOff
provider_slug: takeoff
slug: takeoff-domain-security
source_filename: takeoff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of takeoff.com and its subdomains, 2026-08-29\ndescription: >-\n  Domain security posture for Takeoff Technologies. The registrable domain is\n  well maintained at the DNS layer — it is DNSSEC-signed with a DS record in the\n  parent zone and publishes both SPF and DMARC — but the web tier has decayed:\n  the marketing host www.takeoff.com has no TLS certificate at all, and\n  status.takeoff.com presents a certificate that does not match its hostname.\n  Only the API gateway api.takeoff.com holds a current certificate.\nhosts:\n  - host: api.takeoff.com\n    https: true\n    http_version: 2\n    tls_verified: true\n    cert_subject: CN=api.takeoff.com\n    cert_issuer: 'C=US, O=Google Trust Services, CN=WR3'\n    cert_not_before: Jul 16 12:02:49 2026 GMT\n    cert_expires: Oct 14 12:56:22 2026 GMT\n    hsts: false\n    note: >-\n      Certificate was reissued 2026-07-16, six weeks before this probe —\
  \ the API\n      tier is actively maintained even though the company's marketing site is not.\n  - host: www.takeoff.com\n    https: false\n    error: tls-handshake-failed\n    detail: >-\n      openssl s_client reports \"no peer certificate available\" and SSL alert\n      number 80 (internal error) against 18.211.166.153; the hostname is a CNAME\n      to proxy-ssl.webflow.com / proxy-ssl-geo-2.webflow.com, so the Webflow SSL\n      certificate for this custom domain is no longer provisioned. HTTP on port\n      80 answers 301 to the same unreachable https URL, leaving no reachable\n      web presence.\n    hsts: null\n  - host: takeoff.com\n    https: false\n    error: tls-handshake-failed\n    http_redirect: 'HTTP/1.1 301 -> https://www.takeoff.com/ (X-Cluster-Name: us-east-1-prod-hosting-red)'\n    hsts: null\n  - host: status.takeoff.com\n    https: false\n    error: tls-certificate-name-mismatch\n    detail: >-\n      CNAME to qth8l8vxd7y4.stspg-customer.com (Atlassian Statuspage);\
  \ the\n      presented certificate carries no SAN for status.takeoff.com.\n    hsts: null\ndomains:\n  - domain: takeoff.com\n    dnssec: true\n    dnskey_present: true\n    ds_present: true\n    ds: 13589 8 2 78FC2F68353D880A0302900BAC971A0C5B21300E7340E49852C8CE1A5D1A0BDA\n    caa: []\n    caa_present: false\n    spf: true\n    spf_record: >-\n      v=spf1 a mx include:_spf.google.com include:mail.zendesk.com\n      include:sendgrid.net include:stspg-customer.com ip4:168.245.1.42\n      ip4:149.72.173.189 ip4:149.72.195.148 include:mail.zohopayroll.in ~all\n    dmarc: true\n    dmarc_policy: none\n    dmarc_record: 'v=DMARC1; p=none; rua=mailto:dmarc-reports@takeoff.com'\n    nameservers:\n      - ns-cloud-b1.googledomains.com\n      - ns-cloud-b2.googledomains.com\n      - ns-cloud-b3.googledomains.com\n      - ns-cloud-b4.googledomains.com\n    mx: Google Workspace (aspmx.l.google.com)\nfindings:\n  - No CAA record is published, so any public CA may issue for takeoff.com.\n  - DMARC\
  \ is published at p=none (monitor only), so spoofed mail is reported but not rejected.\n  - HSTS is not set on the one host that completes a TLS handshake.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takeoff/refs/heads/main/security/takeoff-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Grocery
- Retail
- E-Commerce
- Fulfillment
- Micro-Fulfillment
- Warehouse Automation
- Robotics
- Supply Chain
- Logistics
---
