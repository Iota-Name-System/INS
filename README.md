# INS
WARNING!!!
Everything in this document is subject to change!

## Research ENS

Current Schemes for a Wallet name service

The ENS system makes use of the ".eth" TDL:
address_name.eth 
- The power in this is subdomains which allow for use cases such as person.company_name.eth _I think we should stick to that. A hierarchical system is the core functionality of a DNS
- 

### Identified problems
- **Traditional users might not want the URL style naming service**: Ticket2Andromeda is of the opinion that ordinary users perhaps do not want the '.eth' identifier or in our case the '.ins' (Iota Name System) , '.cns' (Crypto Name System - if we're aiming to be the more general NS) or simply '.iota'

Traditional Possible formats

Root Example: Ticket2Andromeda.iota, Ticket2Andromeda.ins, Ticket2Andromeda.cns, Ticket2Andromeda.iota.cns
Sub  Example: Ticket2Andromeda.INS-Team.iota, Ticket2Andromeda.INS-Team.ins, Ticket2Andromeda.INS-Team.iota.cns,

Experimental formats
Left - Right Hierarchal System Example CNS.IOTA.Ticket2Andromeda CNS.IOTA.Ticket2Andromeda.INS-TEAM
But I (Ticket2Andromeda) am a major proponent of using @ to replace CNS.IOTA
as I feel that if users simply want to send crypto to eachother the convention to talk
to one another in the form of a domain name feels... not so satisfying in MY *OPINION*

@gmiasmo: I think we should keep the traditional naming convention, simply because it is the standard. Remember how many problems arose for iota back in 2018 because they tried to reinvent the wheel (ternary instead of binary, WOTS instead of EDS,....). Let's keep stuff simple and therefore also compatible (at least in the base layer). Alternative naming conventions like these:

Root Sym-Example: @Ticket2Andromeda, #Ticket2Andromeda, !Ticket2Andromeda
Sub  Sym-Example: @Ticket2Andromeda.INS-Team, @INS-TEAM.Ticket2Andromeda

can be implmented in the wallet by simple mappings. Again, in my opinion, the hierarchical nature is the key functionality of a DNS. You want the toplevel domain to be exclusive because this allows you also to give different permissions. Like you can only send from a top-level wallet and only receive from lower ones or sth like that.

Our goals should be to make it extremely easy for firefly (and all wallet) IOTA users to be able to send IOTAs amongst one another.
I think  diverging from ".eth",".ins",".iota" paradigm will achieve this. However this will make it slightly less flexible for organizations
that happen to share the same name. 
Microsoft could have a Microsoft.eth or Microsoft.iota for payment 
Or they could simply use @Microsoft, ~Microsoft, !Microsoft, +Microsoft.
This could give use additional flixibility with the capability to use op codes so we can identifity which cryptop were in "iota@Microsoft" , "eth@Microsoft"
and the op code could tell us if the address is an expected CRYPTO WALLET or if its a SMART CONTRACT ADDRESS

@gmiasmo: You are right, flexibility is key but that can be achieved by an adress book or mappings inside the wallet itself. Architecture-wise we NEED a hieracrhical system in my opinion. What kind of separator we use is basically free to choose, but the standard is to use a "." . jon@support@microsoft@iota looks weird imo. For the same reason, I would stick to to the top-down equals right-to-left convention.

@Ticket2Andromeda You're right, absolutely right. It will allow us to remain flexible and focus on optimizing or improving currently existing systems such as ENS. Additionally it gives us the support to host unstoppable domains. So now we should be looking to secure at least unofficially the TLDS of IOTA and CNS and INS. Definitely a fan of allowing a if "@" then add ".iota/ins/cns/" 
##### Design ideas

- *Idea to counter squatting*: Every top-level domain needs to be pledged to a running node, otherwise another user has the right to buy it from the owner for his purchasing price. This guarantees that people are not simply buying up domain names with no intention of ever using them and legit businesses have another incentive to run a node. Sublevel domains can be assigned to wallets without running a node. Imo this is an organic analogy to how it is done in the web.If you run a toplevel domain, you also have to host (or rent) servers. If you are a private person only looking to connect your wallet, a business could offer its toplevel domain and you could have a sublevel domain there without running a node. Similar to email. You open an account at gmail, using their servers as me@gmail.com. The private user does not own gmail.com but gmail does the hosting. Economic incentives in the iota network could be pledging mana, ads in firefly, small fees.....similar to what is done currently with mail providers. 
- @T2A Okay, I'm all aboard on this idea as well. To take this a step further we could possibly increase adoption by reserving the top 500 companies global names and saving them for the TLD, we can also run the TLD of "reddit" temporarily and run a script where everyones reddit usernames auto reserves a subdomain under the TLD reddit and its connected to their username. The top 500 companies and in this strategy it would include reddit, we'd offer them their tokens first over a set time period free but as you said, TLD's are pledged to nodes so they'd have to run a node. BOOM . 
- -*Additional idea*: we could also put a TTL (Time to live) on the tokens not pledges to a node. If after a set period say a month or 90 days who knows, the token will be burned and name will be available to the registry again. 

#####QUESTIONS
T2A to Gmiasmo 
Do we want to be the central 

######**TASKS**
SECURE TLDS
[] IOTA
[] INS
[] CNS

ISCP Familiarity
[] [] Complete Tutorials 

Things to figure out
[] Purpose of Domain Registrar TTL?
[] Onboarding New members
[] Agreement of INS/CNS MISSION, TEAM, RESPONSIBILITY, PURPOSE, COMPENSATION FOR MEMBERS, AND WHATEVER ELSE IS IMPORTANT FOR A TEAM
[] We could become a DAO Decentralized Autonmous Organization
