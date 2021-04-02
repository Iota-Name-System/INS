# INS
WARNING!!!
Everything in this document is subject to change!


Current Schemes for a Wallet name service

The ENS system makes use of the ".eth" TDL:
address_name.eth 
The power in this is subdomains which allow for use cases such as
person.company_name.eth

Ticket2Andromeda is of the opinion that ordinary users perhaps do not want the '.eth' identifier or 
in our case the '.ins' (Iota Name System) , '.cns' (Crypto Name System - if we're aiming to be the more general NS) or simply
'.iota'

Traditional Possible formats

Root Example: Ticket2Andromeda.iota, Ticket2Andromeda.ins, Ticket2Andromeda.cns, Ticket2Andromeda.iota.cns
Sub  Example: Ticket2Andromeda.INS-Team.iota, Ticket2Andromeda.INS-Team.ins, Ticket2Andromeda.INS-Team.iota.cns,

Experimental formats
Left - Right Hierarchal System Example CNS.IOTA.Ticket2Andromeda CNS.IOTA.Ticket2Andromeda.INS-TEAM
But I (Ticket2Andromeda) am a major proponent of using @ to replace CNS.IOTA
as I feel that if users simply want to send crypto to eachother the convention to talk
to one another in the form of a domain name feels... not so satisfying in MY *OPINION*

Root Sym-Example: @Ticket2Andromeda, #Ticket2Andromeda, !Ticket2Andromeda
Sub  Sym-Example: @Ticket2Andromeda.INS-Team, @INS-TEAM.Ticket2Andromeda

Our goals should be to make it extremely easy for firefly (and all wallet) IOTA users to be able to send IOTAs amongst one another.
I think  diverging from ".eth",".ins",".iota" paradigm will achieve this. However this will make it slightly less flexible for organizations
that happen to share the same name. 
Microsoft could have a Microsoft.eth or Microsoft.iota for payment 
Or they could simply use @Microsoft, ~Microsoft, !Microsoft, +Microsoft.
This could give use additional flixibility with the capability to use op codes so we can identifity which cryptop were in "iota@Microsoft" , "eth@Microsoft"
and the op code could tell us if the address is an expected CRYPTO WALLET or if its a SMART CONTRACT ADDRESS
