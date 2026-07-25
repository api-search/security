---
api_specs:
- filename: amazon-codeartifact-authorization-token-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Authorization Token#domain API
  slug: amazon-codeartifact-authorization-token-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-authorization-token-domain-api-openapi.yml
- filename: amazon-codeartifact-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domain API
  slug: amazon-codeartifact-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domain-api-openapi.yml
- filename: amazon-codeartifact-domain-domain-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domain#domain API
  slug: amazon-codeartifact-domain-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domain-domain-api-openapi.yml
- filename: amazon-codeartifact-domains-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Domains API
  slug: amazon-codeartifact-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-domains-api-openapi.yml
- filename: amazon-codeartifact-package-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Package API
  slug: amazon-codeartifact-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-package-api-openapi.yml
- filename: amazon-codeartifact-package-domain-repository-format-package-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Package#domain&repository&format&package API
  slug: amazon-codeartifact-package-domain-repository-format-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-package-domain-repository-format-package-api-openapi.yml
- filename: amazon-codeartifact-packages-domain-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Packages#domain&repository API
  slug: amazon-codeartifact-packages-domain-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-packages-domain-repository-api-openapi.yml
- filename: amazon-codeartifact-repositories-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repositories API
  slug: amazon-codeartifact-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repositories-api-openapi.yml
- filename: amazon-codeartifact-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repository API
  slug: amazon-codeartifact-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repository-api-openapi.yml
- filename: amazon-codeartifact-repository-domain-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Repository#domain&repository API
  slug: amazon-codeartifact-repository-domain-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-repository-domain-repository-api-openapi.yml
- filename: amazon-codeartifact-tag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tag#resourceArn API
  slug: amazon-codeartifact-tag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tag-resourcearn-api-openapi.yml
- filename: amazon-codeartifact-tags-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Tags#resourceArn API
  slug: amazon-codeartifact-tags-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-tags-resourcearn-api-openapi.yml
- filename: amazon-codeartifact-untag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon CodeArtifact Untag#resourceArn API
  slug: amazon-codeartifact-untag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/openapi/amazon-codeartifact-untag-resourcearn-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: codeartifact.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Codeartifact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon CodeArtifact, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
slug: amazon-codeartifact-domain-security
source_filename: amazon-codeartifact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: codeartifact.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/security/amazon-codeartifact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
---
