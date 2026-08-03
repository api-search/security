---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sourcebooks.com
  spf: true
- caa: []
  caa_note: apex is a CNAME to dnejtelqn5d5p.cloudfront.net, so no CAA record is served
  dmarc: false
  dnssec: false
  domain: callistopublishing.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:it-dmarc@callistomedia.com
  dnssec: false
  domain: callistomedia.com
  mx: true
  mx_note: callistomedia-com.mail.protection.outlook.com — the legacy mail domain is still live on Microsoft 365 even though the website is gone
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Oct  5 12:07:30 2026 GMT
  host: www.sourcebooks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.callistopublishing.com
  hsts: false
  https: true
  redirects_to: https://www.sourcebooks.com/callisto/
  tls_version: TLSv1.3
- host: callistomedia.com
  hsts: false
  https: false
  https_note: TCP connect to port 443 timed out on 2026-08-02; HTTP port 80 answers 301 to https://www.callistopublishing.com
  redirects_to: https://www.callistopublishing.com
kind: domain-security
layout: security
method: probed
name: Callisto Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callisto Media, probed live across 3 host(s) and 3 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Callisto Media
provider_slug: callisto-media
slug: callisto-media-domain-security
source_filename: callisto-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the legacy Callisto Media domains\nnotes: 'Callisto Media has no host of its own. callistomedia.com serves only an HTTP\n  301 to callistopublishing.com (port 443 does not answer), callistopublishing.com\n  is a CloudFront CNAME that 301s to sourcebooks.com/callisto, and www.sourcebooks.com\n  is the Sourcebooks storefront that now carries the Callisto brand. Absence of a record\n  is recorded as observed, not inferred.'\nhosts:\n- host: www.sourcebooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:07:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.callistopublishing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n  redirects_to: https://www.sourcebooks.com/callisto/\n- host: callistomedia.com\n  https: false\n  https_note: TCP connect to port 443 timed out on 2026-08-02; HTTP port 80 answers\n\
  \    301 to https://www.callistopublishing.com\n  hsts: false\n  redirects_to: https://www.callistopublishing.com\ndomains:\n- domain: sourcebooks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: callistopublishing.com\n  dnssec: false\n  caa: []\n  caa_note: apex is a CNAME to dnejtelqn5d5p.cloudfront.net, so no CAA record is served\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: false\n- domain: callistomedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; rua=mailto:it-dmarc@callistomedia.com\n  mx: true\n  mx_note: callistomedia-com.mail.protection.outlook.com — the legacy mail domain is\n    still live on Microsoft 365 even though the website is gone\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callisto-media/refs/heads/main/security/callisto-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Publishing
- Book Publishing
- Educational Publishing
- Children's Books
- Nonfiction
- Media
- Consumer Products
- Data-Driven Publishing
- Acquired
- United States
---
