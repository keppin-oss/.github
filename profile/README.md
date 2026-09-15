# Keppin-OSS

Security and identity building blocks for Go, Windows, and OpenZiti.

Keppin-OSS provides focused, reusable components for machine-bound identity,
non-exportable key custody, secure local communication, and OpenZiti integration.

## Projects

### [CNG](https://github.com/keppin-oss/cng)

Windows CNG/KSP machine-key custody for Go applications.

Use machine-scoped, non-exportable private keys through Go's standard
`crypto.Signer` model without exporting private key material.

**Status:** Available — `v0.1.2`

---

### [OpenZiti-CNG](https://github.com/keppin-oss/openziti-cng)

OpenZiti integration for Windows CNG/KSP-backed non-exportable machine identities.

Connects OpenZiti's identity engine and native enrollment flow to keys managed
by Keppin-OSS CNG.

**Status:** Available — `v0.1.2`

---

### [Enterprise TLS](https://github.com/keppin-oss/enterprise-tls)

TLS infrastructure for enterprise-managed application deployments.

**Status:** Available — `v0.1.1`

---

### [Machine Identity](https://github.com/keppin-oss/machine-identity)

Machine-bound identity primitives for applications and services.

**Status:** Available — `v0.1.0`

---

### [Local TLS](https://github.com/keppin-oss/local-tls)

TLS infrastructure for secure local application communication.

**Status:** Available — `v0.1.1`


## Design principles

Keppin-OSS projects are designed around a few core principles:

- keep private key material inside the platform cryptographic provider where supported;
- make trust boundaries explicit;
- expose small, reusable Go modules instead of application-specific frameworks;
- integrate with existing security protocols rather than reimplementing them;
- keep the open-source components independent from Keppin-Suite.

## Ecosystem

The modules are designed to compose rather than form a monolithic runtime.

As the remaining projects are published, this page will document their
relationships and the supported integration paths.

---

Keppin-OSS is maintained by [AxelConsulting](https://github.com/AxelConsulting).
