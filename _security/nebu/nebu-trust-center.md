---
certifications: []
description: ''
kind: trust-center
layout: security
name: Nebu Trust Center
name_suffix: Trust Center
overview: Nebu maintains a public trust center covering its security and compliance posture.
provider_name: Nebu
provider_slug: nebu
slug: nebu-trust-center
source_filename: nebu-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nprobe: true\nsource: https://thenebu.com/.well-known/security.txt\nurl: null\nnote: >-\n  NEBU has no dedicated trust-center page. thenebu.com is a single-page marketing\n  site whose CloudFront catch-all returns the homepage for every path, so a probe\n  of /trust matched compliance keywords from the homepage rather than a real page.\n  The certification/compliance CLAIMS below are, however, genuinely self-published\n  by NEBU: in the homepage schema.org SoftwareApplication featureList and in the\n  Security Commitments section of /.well-known/security.txt. They are self-asserted\n  marketing claims (SOC 2 stated as \"Type II Ready\", i.e. not yet attested), not\n  independently verified certifications, and no audit reports or trust portal were\n  found. No `Compliance` pointer is emitted on the strength of these claims alone.\ncertifications_claimed:\n- name: SOC 2 Type II\n  status: ready (self-stated, not yet attested)\n- name:\
  \ ISO 27001\n  status: certified (self-stated)\n- name: GDPR\n  status: compliant (self-stated)\nevidence:\n- source: https://thenebu.com/.well-known/security.txt\n  kind: security.txt Security Commitments section\n  keywords:\n  - SOC 2 Type II Ready\n  - ISO 27001 Certified\n  - GDPR Compliant\n- source: https://thenebu.com/\n  kind: schema.org SoftwareApplication featureList (JSON-LD)\n  keywords:\n  - SOC2 compliance ready\n  - ISO 27001 certified\n  - GDPR compliant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nebu/refs/heads/main/security/nebu-trust-center.yml
summary_line: trust center published
tags:
- Company
- DevOps
- Cloud
- Artificial Intelligence
- AIOps
- MLOps
- Cloud Management
- Automation
- Cost Optimization
trust_url: ''
---
