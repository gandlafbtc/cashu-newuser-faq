            **CASHU - NEW USER FREQUENTLY ASKED QUESTIONS (FAQs)
**TUTORIALS**

BTC Sessions-Cashu and Nutstash Wallets: https://www.youtube.com/watch?v=riTRD0BdMDI

**MINTS**

CAUTION: Choose Mints where you trust or know and trust the operator.  If you don't trust the mint, use small amounts or immediately redeem tokens or swap tokens to your own mint(??good rec??).

Q: Why can't I receive tokens from one mint into another mint or my own mint?

A: You cannot receive tokens from one mint into another mint.  To transfer tokens from one mint to another, use the Intermint Swap functionality. 

Q: How to I send (swap) tokens from one mint to another?

A: Use Intermint Swap functionality, which operates via Lightning invoices under the hood.
   * Cashu.me - go to the Settings tab.
   * Nutstash - go to the Mint tab. 


Note: You must have 2 mints in order to send/swap between mints.

Q: Is there a list of mints?

A: Listing mints would imply trust and recommendation of a mint.  There are 2 test mints:
    * Cashu.me - https://8333.space:3338
    * Nutstash - https://legend.lnbits.com/cashu/api/v1/4gr9Xcmz3XEkUNwiBiQGoC

Q: How do I set up my own mint?

A: The easiest way to set up your own mint is in LNBits Cashu on the legends.lnbits.com server or on your own LNBits instance. You can also set up your own mint via the Nutshell tool--see Github for instructions.

**RECEIVING TOKENS**

Q: What if I do not want to trust a mint and receive to a Nutstash, Cashu.me, or other wallet?

A: You can redeem your tokens immediately via Lightning invoice on: https://redeem.cashu.me/

**WALLETS**
    
CAUTION: Do not open the same wallet in multiple browser tabs.
. 
Q: I have had pending tokens for quite some time, how do I resolve this?

A: You can receive the tokens back to your own wallet. Check the History for the token to receive back into your wallet.

Q: Do invoices generated from Cashu or Nutstash expire?

A: This varies depending on the mint. 

**WALLET BACKUPS**
CAUTION:VYour current backup is invalid if you make additional transactions.  Re-do the backup to get a backup of current wallet state.

Q: How do I make a backup?

A: In Nutstash, on the Settings page.  In Cashu.me (Heidi,try this out)

Q: Why can't I restore my cashu.me backup into Nutstash? 

A: Wallet backups are only for that particular wallet implementation. To move your ecash to another wallet implementation, send the ecash from wallet to wallet or via Lightning withdrawal and minting.

**NOSTR**

Nutstash: Go to the Settings tab to configure Nostr. Use an external key or generate throwaway nostr keys. When you send tokens, you can then specify a Nostr pubkey.

Nutshell: Follow the Github instructions to configure Nostr by editing the .env file, then send tokens to a Nostr pubkey.

****GENERAL PRIVACY QUESTIONS****

Q: How does the Cashu ecash protocol implement privacy?

A: See http://lconf.gandlaf.com or (Heidi find Adopting Lightning Calle preso) for an introduction to the Cashu protocol. Or read the Cashu NUTs (Notation, Usage, Terminology) in Github here: https://github.com/cashubtc/nuts

Q: Are there user accounts in the Cashu protocol?

A: No.

Q: Can the Mint see my IP address when I use Nutstash or Cashu.me Web wallets?

A: If you are not using Tor or a VPN, the Mint could see your IP address.

Q: Can I use Tor with Nutstash and Cashu.me Web wallets?

A: To use Tor with Nutstash or Cashu.me, you need to Remember History and set up an exception in Manage Exceptions for the checked Delete cookies and site data when Tor Browser is closed. 
When using Nutshell, Tor is started if your .env file has set the setting TOR=TRUE.

Q: Are mints able to track ecash wallets by storing the payment_hash when a user receives a Lightning payment?

A: No, the mint does not know the Cashu ecash secret or unblinded signature (see Nut-0 in Github https://github.com/cashubtc/nuts/blob/main/00.md). Therefore, there is no linkability between a Lightning invoice and Cashu ecash.  

