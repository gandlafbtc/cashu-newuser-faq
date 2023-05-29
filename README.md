# CASHU - FREQUENTLY ASKED QUESTIONS (FAQs)

![alt text](https://github.com/findingsov/cashu-newuser-faq/blob/main/CashuImg.png "Logo Title Text 1")

## TUTORIALS

BTC Sessions-Cashu and Nutstash Wallets: https://www.youtube.com/watch?v=riTRD0BdMDI

If you want to use this FAQ in https://chatpdf.com, simply drag the cashu-newuser-faq
.pdf file to the chatPDF site.

**CAUTION**: Use small amounts on all mints.

## MINTS

**CAUTION:** Choose Mints where you trust or know and trust the operator.  Use small amounts or immediately redeem tokens or swap tokens to your own mint.

### Q: Why can't I receive tokens from one mint into another mint or my own mint?

A: You cannot receive tokens from one mint into another mint.  To transfer tokens from one mint to another, use the Intermint Swap functionality. 

### Q: How to I send (swap) tokens from one mint to another?

A: Use Intermint Swap functionality, which operates via Lightning invoices under the hood.

* Cashu.me - go to the Settings tab.
* Nutstash - go to the Mint tab. 


Note: You must have 2 mints in order to send/swap between mints.

### Q: Is there a list of mints?

A: There are 2 test mints: 

* Cashu.me - https://8333.space:3338 
* Nutstash - https://legend.lnbits.com/cashu/api/v1/4gr9Xcmz3XEkUNwiBiQGoC 

You can see the complete list of mints here: https://mintindex.gandlaf.com 

### Q: How do I set up my own mint?

A: The easiest way to set up your own mint is in LNbits Cashu on the legends.lnbits.com server or on your own LNbits instance. You can also set up your own mint via the Nutshell tool--see Github for instructions.

### Q: Can I send and receive tokens to/from the same mint?

A: Yes, this is a common first test use case.  Also, sometimes you might send a token that is not received or redeemed, and you might want to copy the token and receive it back to yourself.


## RECEIVING TOKENS

### Q: What if I do not want to trust a mint and receive to a Nutstash, Cashu.me, or other wallet?

A: You can redeem your tokens immediately via Lightning invoice on: https://redeem.cashu.me/

## WALLETS
    
**CAUTION:** Do not open the same wallet in multiple browser tabs.
 
### Q: I have had pending tokens for quite some time, how do I resolve this?

A: You can receive the tokens back to your own wallet. Check the History for the token to receive back into your wallet.

### Q:  Can I get a QR code for a token?

A: In Cashu.me, if you send a token that is a power of 2, you will see a QR code (e.g., 2, 4, 8, 16, 32, 64, 128, etc). This is because only 1 token can fit in a QR code.

### Q: Do invoices generated from Cashu or Nutstash expire?

A: This varies depending on the mint. 

## WALLET BACKUPS

**CAUTION:** Your current backup is invalid if you make additional transactions.  Re-do the backup to get a backup of current wallet state.

### Q: How do I make a backup and restore?
A:  Backup and restore mechanisms are specific to each particular wallet.

* Nutstash - go to the Settings tab. 
* Cashu.me - go to the Welcome page and make a Backup.  You can then open a new browser and drop the Backup JSON file on the Welcome screen.  


### Q: Why can't I restore my cashu.me backup into Nutstash? 

A: Wallet backups are only for that particular wallet implementation. To move your ecash to another wallet implementation, send the ecash from wallet to wallet or via Lightning withdrawal and minting.

## NOSTR

### Q: How do I configure nostr?

A:  For Nutstash: Go to the Settings tab to configure Nostr. Use an external key or generate throwaway nostr keys. When you send tokens, you can then specify a Nostr pubkey. 
    For Nutshell: Follow the Github instructions to configure Nostr by editing the .env file, then send tokens to a Nostr pubkey.

## GENERAL PRIVACY QUESTIONS

### Q: How does the Cashu ecash protocol implement privacy?

A: See http://lconf.gandlaf.com or https://www.youtube.com/watch?v=UNjVc-WYdgE&t=105s for an introduction to the Cashu protocol. Or read the Cashu NUTs (Notation, Usage, Terminology) in Github here: https://github.com/cashubtc/nuts

### Q: Are there user accounts in the Cashu protocol?

A: No.

### Q: Can the Mint see my IP address when I use Nutstash or Cashu.me Web wallets?

A: If you are not using Tor or a VPN, the Mint could see your IP address.

### Q: Can I use Tor with Nutstash and Cashu.me Web wallets?

A: To use Tor with Nutstash or Cashu.me, you need to Remember History and set up an exception in Manage Exceptions for the checked Delete cookies and site data when Tor Browser is closed. 
When using Nutshell, Tor is started if your .env file has set the setting TOR=TRUE.

### Q: Are mints able to track ecash wallets by storing the payment_hash when a user receives a Lightning payment?

A: No, the mint does not know the Cashu ecash secret or unblinded signature (see Nut-0 in Github https://github.com/cashubtc/nuts/blob/main/00.md). Therefore, there is no linkability between a Lightning invoice and Cashu ecash.  

## UPDATING

### Q: How do I update Cashu when LNBits or Cashu on LNBits have an update?
A:  First, download a current Cashu wallet backup as a precaution.
LNbits: To update LNBits, follow the update instructions here:
https://github.com/lnbits/lnbits/wiki/LNbits-Documentation#install-options

Cashu: To re-install (after LNbits update) or update Cashu, follow the update instructions here:
https://github.com/lnbits/lnbits/wiki/LNbits-Extensions
    