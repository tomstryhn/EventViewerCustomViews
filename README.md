# Event Viewer Custom Views

Custom Views for Microsoft Windows Event Viewer

## Table of Content
  - [Background](#background)
  - [How to Use](#how-to-use)
  - [Custom Views](#custom-views)
     - [Account Authentication](#account-authentication)
     - [Administrator Logon (Failed)](#administrator-logon-failed)
     - [Administrator Logon (Successful)](#administrator-logon-successful)
     - [Legacy Kerberos Ticket Encryption Types](#legacy-kerberos-ticket-encryption-types)
     - [Logon (Failed)](#logon-failed)
     - [Logon (Successful)](#logon-successful)
     - [NTLMv1 Authentications](#ntlmv1-authentications)
     - [Security Group Membership](#security-group-membership)
     - [Security Group Membership](#security-group-membership)
     - [Security Group Membership](#security-group-membership)
     - [Service Creation](#service-creation)
     - [Service Creation Error](#service-creation-error)
     - [User Creation](#user-creation)

## Background
I often find myself using the Microsoft Event Viewer when gathering information related to hardening tasks in Windows Environments, troubleshooting or gathering data when doing forensic work. There's many ressources online for ie. XML filters when filtering in the EventLogs, these are often used together with the *Custom Views* in the *Event Viewer*. So I started gathering these filters, and created these *templates*, so I quickly can download the XML-file and use the builtin *Import Custom View...* feature inside the *Microsoft Event Viewer*.

## How to Use
Find the Custom View in the list, download it to the computer, or copy the content to Notepad and save the file as an ```.xml```, then open *Event Viewer*, right click on the *Custom Views* in the top left pane, and select *Import Custom View...*

## Custom Views
#### Account Authentication
   - Successful and Failed Account Authentication <br />
      - XMLFile: [00D111.xml](./xml/00D111.xml)
#### Administrator Logon (Failed)
   - Failed Administrator Account Logons <br />
      - XMLFile: [01D97C.xml](./xml/01D97C.xml)
#### Administrator Logon (Successful)
   - Successful Administrator Account Logons <br />
      - XMLFile: [42F217.xml](./xml/42F217.xml)
#### Legacy Kerberos Ticket Encryption Types
   - Legacy Kerberos Ticket Encryption Types: DES-CBC-CRC, DES-CBC-MD5, RC4-HMAC, RC4-HMAC-EXP <br />
      - XMLFile: [049517.xml](./xml/049517.xml)
#### Logon (Failed)
   - Failed Account Logons <br />
      - XMLFile: [F222E4.xml](./xml/F222E4.xml)
#### Logon (Successful)
   - Successful Account Logons <br />
      - XMLFile: [380759.xml](./xml/380759.xml)
#### NTLMv1 Authentications
   - NTLMv1 (Windows New Technology LAN Manager) Authentications <br />
      - XMLFile: [0226D5.xml](./xml/0226D5.xml)
#### Security Group Membership
   - Member added to Security Group (Local Group) <br />
      - XMLFile: [86F11C.xml](./xml/86F11C.xml)
#### Security Group Membership
   - Member added to Security Group (Universal Group) <br />
      - XMLFile: [BA131A.xml](./xml/BA131A.xml)
#### Security Group Membership
   - Member added to Security Group (Global Group) <br />
      - XMLFile: [C86A1B.xml](./xml/C86A1B.xml)
#### Service Creation
   - Service Creation <br />
      - XMLFile: [A82979.xml](./xml/A82979.xml)
#### Service Creation Error
   - Service Creation Errors <br />
      - XMLFile: [A57B21.xml](./xml/A57B21.xml)
#### User Creation
   - User Creation <br />
      - XMLFile: [0495E8.xml](./xml/0495E8.xml)
