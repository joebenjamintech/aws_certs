# KMS

- KMS - key managment service - creates and manage encryption keys for a variety of AWS services or for your apps
- can be used with cloudtrail to audit keys access history
- has the ability to automatically rotate out your keys every year with no need to re-encrypt
- CMK - customer master keys - are the primary resources in KMS
- KMS is a multi-tenant HSM, multi-tenant means you are sharing the hardware with multiple customers
- HSM - hardware security model - is a specialized hardware for storing your keys and a tamper proof
- KMS is up to FIPS 140-2 level 2 compliant
- KMS stores master keys (not data keys)
- master keys are used to encrypt data keys which is called envelop encryption
- KMS supports two types of keys symmetric and assymetric
  - symmetric is a single key using 256 bit encryption eg. S3 bucket AES-256
  - assymetric - uses two keys, eg. key pair public and private
- important KMS APIS to remember
  - aws kms create-key --creates a key
  - aws kms encrypt --encryps a key
  - aws kms decrypt - decrypts a key
  - aws kms recrypt - re-encrypts a key
  - aws kms enable-key-rotation --turn on autmoatic key rotation (only for symmetric keys)
