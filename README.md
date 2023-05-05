<h1>CASHU - NEW USER FREQUENTLY ASKED QUESTIONS (FAQs)</h1>

![alt text](https://github.com/findingsov/cashu-newuser-faq/blob/main/CashuImg.png "Logo Title Text 1")

<h2>TUTORIALS</h2>

BTC Sessions-Cashu and Nutstash Wallets: https://www.youtube.com/watch?v=riTRD0BdMDI

<h2>MINTS</h2>

<b>CAUTION:</b> Choose Mints where you trust or know and trust the operator.  If you don't trust the mint, use small amounts or immediately redeem tokens or swap tokens to your own mint.

<h3>Q: Why can't I receive tokens from one mint into another mint or my own mint?</h3>

A: You cannot receive tokens from one mint into another mint.  To transfer tokens from one mint to another, use the Intermint Swap functionality. 

<h3>Q: How to I send (swap) tokens from one mint to another?</h3>

A: Use Intermint Swap functionality, which operates via Lightning invoices under the hood.
<ul>
    <li> Cashu.me - go to the Settings tab.</li>
     <li> Nutstash - go to the Mint tab. </li>
</ul>

Note: You must have 2 mints in order to send/swap between mints.

<h3>Q: Is there a list of mints?</h3>

A: Listing mints would imply trust and recommendation of a mint.  There are 2 test mints:
<ul>
    <li> Cashu.me - https://8333.space:3338 </li>
     <li>Nutstash - https://legend.lnbits.com/cashu/api/v1/4gr9Xcmz3XEkUNwiBiQGoC </li>
</ul>
<h3>Q: How do I set up my own mint?</h3>

A: The easiest way to set up your own mint is in LNBits Cashu on the legends.lnbits.com server or on your own LNBits instance. You can also set up your own mint via the Nutshell tool--see Github for instructions.

<h2>RECEIVING TOKENS</h2>

<h3>Q: What if I do not want to trust a mint and receive to a Nutstash, Cashu.me, or other wallet?</h3>

A: You can redeem your tokens immediately via Lightning invoice on: https://redeem.cashu.me/

<h2>WALLETS</h2>
    
<b>CAUTION:</b> Do not open the same wallet in multiple browser tabs.
 
<h3>Q: I have had pending tokens for quite some time, how do I resolve this?</h3>

A: You can receive the tokens back to your own wallet. Check the History for the token to receive back into your wallet.

<h3>Q: Do invoices generated from Cashu or Nutstash expire?</h3>

A: This varies depending on the mint. 

<h2>WALLET BACKUPS</h2>

<b>CAUTION:</b> Your current backup is invalid if you make additional transactions.  Re-do the backup to get a backup of current wallet state.

<h3>Q: How do I make a backup and restore?</h3>
A:  Backup and restore mechanisms are specific to each particular wallet.
<ul>
     <li> Nutstash - go to the Settings tab. </li>
     <li> Cashu.me - At this time, you can download a backup and restore via Developer Tools.  A backup/restore mechanism is a work in progress.
</ul>

<h3>Q: Why can't I restore my cashu.me backup into Nutstash? </h3>

A: Wallet backups are only for that particular wallet implementation. To move your ecash to another wallet implementation, send the ecash from wallet to wallet or via Lightning withdrawal and minting.

<h2>NOSTR</h2>

<h3>Q: How do I configure nostr?</h3>

A:  For Nutstash: Go to the Settings tab to configure Nostr. Use an external key or generate throwaway nostr keys. When you send tokens, you can then specify a Nostr pubkey. 
    For Nutshell: Follow the Github instructions to configure Nostr by editing the .env file, then send tokens to a Nostr pubkey.

<h2>GENERAL PRIVACY QUESTIONS</h2>

<h3>Q: How does the Cashu ecash protocol implement privacy?</h3>

A: See http://lconf.gandlaf.com or https://www.youtube.com/watch?v=UNjVc-WYdgE&t=105s for an introduction to the Cashu protocol. Or read the Cashu NUTs (Notation, Usage, Terminology) in Github here: https://github.com/cashubtc/nuts

<h3>Q: Are there user accounts in the Cashu protocol?</h3>

A: No.

<h3>Q: Can the Mint see my IP address when I use Nutstash or Cashu.me Web wallets?</h3>

A: If you are not using Tor or a VPN, the Mint could see your IP address.

<h3>Q: Can I use Tor with Nutstash and Cashu.me Web wallets?</h3>

A: To use Tor with Nutstash or Cashu.me, you need to Remember History and set up an exception in Manage Exceptions for the checked Delete cookies and site data when Tor Browser is closed. 
When using Nutshell, Tor is started if your .env file has set the setting TOR=TRUE.

<h3>Q: Are mints able to track ecash wallets by storing the payment_hash when a user receives a Lightning payment?</h3>

A: No, the mint does not know the Cashu ecash secret or unblinded signature (see Nut-0 in Github https://github.com/cashubtc/nuts/blob/main/00.md). Therefore, there is no linkability between a Lightning invoice and Cashu ecash.  

<h2>UPDATING</h2>

<h3>Q: How do I update Cashu when LNBits or Cashu on LNBits have an update?</h3>
A:  First, download a current Cashu wallet backup as a precaution.
LNbits: To update LNBits, follow the update instructions here:
https://github.com/lnbits/lnbits/wiki/LNbits-Documentation#install-options

Cashu: To re-install (after LNbits update) or update Cashu, follow the update instructions here:
https://github.com/lnbits/lnbits/wiki/LNbits-Extensions
    

