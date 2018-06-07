---
title: General Security Considerations for Crypto Currency Exchange
abbrev: General Security Considerations for Crypto Currency Exchange
docname: draft-nakajima-crypto-currency-exchange-security-considerations-latest
category: info
date: {DATE}

ipr: trust200902
area: General
workgroup: saag
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: M. Sato
    name: Masashi Sato
    organization: SECOM CO.,LTD.

 -
    ins: H. Nakajima
    name: Hirotaka Nakajima
    organization: Mercari, Inc.
    email: nunnun@mercari.com

normative:
  RFC2119:

informative:

--- abstract

<!-- この文書は仮想通貨交換所の事業者が利用者の資産を保護する目的としてセキュリティを検討するための推奨事項を整理するものである。保護すべき資産のうち、特に仮想通貨の秘密鍵は従来の情報システムとは異なる特徴があり留意が必要である。仮想通貨交換事業者が秘密鍵を適切に管理し、顧客が意図しない不正な取引を防止するために留意すべき点を特に重点的に述べる。 -->

This document discusses the threat, risk, and controls on the followings;
- Online system of crypto currency exchange that provides the exchange service to its customer (consumers and trade partners);
- Asset information (including the private key of the crypto currency) that the online system of a crypto currency exchange manages;
- Social impact that can arise from the discrepancy in the security measures that are implemented in the online system of a crypto currency exchange.

This document is applicable to the crypto currency exchanges that manages the private key that corresponds to the crypto currency. It includes the organizations that outsources the key management to another organization. In such a case, the certain recommendations applies to those outsourcers.

--- middle

# Introduction

TODO Introduction

# Scope of this document

<!-- 本書が対象とする事業者は、仮想通貨の秘密鍵を保有する仮想通貨交換所の事業者である。秘密鍵の管理を他の事業者へ委託する場合も含む。その場合、秘密鍵の管理を委託された事業者についても、本書が示す推奨事項の相当箇所が適用されるものと考える。
本書は以下の対象に対する脅威やリスクに関する考察を含む。
顧客（消費者や取引相手）に対して仮想通貨の交換業務を提供する仮想通貨交換所オンラインシステム
仮想通貨交換所オンラインシステムが管理する資産情報（仮想通貨の秘密鍵を含む）
仮想通貨交換所オンラインシステムのセキュリティ対策の不備により及ぼしうる社会的な影響
本書で対象とする仮想通貨交換所オンラインシステムの基本モデルは5章で示す。この基本モデルとは別の形態のシステム、例えば、利用者が提示する秘密鍵を事業者が管理する業態（例：オンラインウォレット）等については別の補完的な文書あるいは本書の後の改訂で扱うものとする。
本書は以下についてはスコープ外とする。
仮想通貨の仕組みを提供するブロックチェーンや分散台帳自体に対するセキュリティ対策
事業者自身の経営リスク
顧客と交換所の資産の分離に関する具体的な要件 -->

In this document, virtual currency exchange operators which hold a private key of virtual currency.

# Conventions and Definitions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this
document are to be interpreted as described in BCP 14 {{RFC2119}} {{!RFC8174}}
when, and only when, they appear in all capitals, as shown here.

# Terminology

- Wallet
- Fork of blockchain

# Basic description of a model online system of a crypto currency exchange

## General

In this clause, a model online system of a crypto currency exchange that is used to explain the concepts and provisions in this document are explained.



## A basic model of online system of a crypto currency exchange and its functional components

Followings are the basic model of a crypt currency exchange that this document deals with.

## The flow leading to the sending of the transaction

## Types of keys that are used for signature and encryption

### Type of keys

### A flow for the key generation and the key usage

### On the usage of multiple keys

### On the suspension of keys

## On the characteristics of crypto currency on Blockchain and distributed ledger technologies

### General

### The importance of the private key used for signing

### Diversity of implementations

#### On the cryptographic algorithms used by crypto currencies

#### On the possibility of the forking of the Blockchain

#### Rollback by reorganization

#### The treatment of the forked crypto currencies

### Risk on the unapproved transactions

#### General

#### The handling of the unapproved transactions

#### Transaction failures caused by the vulnerabilities of the implementation or the specification of the crypto currency

# Basic objectives for the security management of crypto currency exchanges

# Approaches to basic security controls

# Sector specific security management controls for crypto currency exchanges

## General

## On the direction of the information security management

## On the controls for key recovery

## On the controls against theft and leakage of the private key for signing

## On the illegal operation of the private key for signing

## On the illegal operation against the asset data

## On the user authentication

## On the withdrawal of the coins

## On the transfer of the crypto currency to an unused address

# Remaining issues

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.

--- back

# Contributors
