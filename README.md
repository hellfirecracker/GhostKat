![alt text](https://i.imgur.com/KqVTrI0.png "GKEKO")

# 0: Return To
The internet is impossible to regulate by nature. It seems controlled through ad gateways and user tracking, but at any point users can circumvent corporations and even governments. They simply need to connect directly to one another.


# 1: GhostKat’s Media Haven 
## (is [WebTorrent](https://webtorrent.io/) + [Ethereum](https://ethereum.org/) Shipping)
  GhostKat is a straightforward method for streaming media 'peer2peer' between viewers, without them needing any special software, torrent websites, or even a server to store file data. **In fact, there is no server supporting GhostKat at all.** Even in a world where net neutrality were dead, GhostKat can circumvent all means of corporate control. This is the start of a migration to a haven protected from any outside authoritarian intervention. 
  
  
  [GhostKat.org](https://www.ghostkat.org) serves a static html page with JavaScript that lets you find other people watching GhostKat. Anyone watching GhostKat is also broadcasting what they are watching to everyone else, also watching. It's a distributed, communistic, and globally available protocol for transferring media. GhostKat never hosts any file data, and never communicates with the viewer's device at all. It's like we hardly exist. **GhostKat is immortal, unblockable, one hundred percent client-side, and can move through walls.**


   It is impossible to remove the file data broadcasted on GK; our website does nothing, it's a static html server. The code it contains runs in the viewer's browser and calls a public decentralized database stored on Ethereum. That database is a list of all the files people are sharing over GhostKat. The basic HTML page then becomes populated with the file names, and when you click on one, we use WebTorrent to connect you with everyone watching that file. 
   
   
   *Our all-in-one html source is all that's needed to run a local version of GK, or spawn endless copies across the world wide web.* The system is in no way dependant on our .org. We highly encourage improving and kustomizing our basic interface. We have posted one example video to a public tier in our database, and you can watch it on GhostKat right Meow!
  

# 2: GhostKat Groove
  It is exteremely easy to replicate what we've done. If you want to, just follow these steps.
We use [Ethereum](https://ethereum.org/) to store the file references  


*Our Kontracts are written in Solidity (C for Ethereum), and are secured by an Ethereum ERC20 Standard Token we call "Dubloonz". Ownership of Dubloonz gives users access to different levels of trust within the database. This Token Access system is cryptographically secure to the highest degree simply by using the Ethereum ERC20 Token Standard.*. 

```C#
string[] public katKafe;
function katPost (string postin) public {
    require(!frozenAccount[msg.sender]);
    require(balanceOf[msg.sender] >= 27);
    katKafe.push(postin);   
}
```
 **This posts a magnet link to each of the hundreds of thousands of Ethereum nodes across the world.** 
 So long as one of those nodes is around, so will our illicit torrent database. Even the Ethereum organization can't remove our database contract. Next, We use [Infura](https://infura.io/) to let the user query Ethereum client-side, in browser.

```javascript
web3 = new Web3(new Web3.providers.HttpProvider("https://mainnet.infura.io/Anzdw8JKc1qLD0QdZBQE"));
var Gkon = web3.eth.contract([insertABI])
var Kontract = Gkon.at("0xF3fEAA67700E31955f3aC95a2d976dc42AAc332A");
```

Finally, we use [WebTorrent](https://webtorrent.io/) as our client-side, in-browser, media streaming client. It is the backbone of GhostKat. It allows users to stream media to each other, rather than from a server.
Our rudimentary HTML interface is being served at [GhostKat.org](https://www.ghostkat.org)
The domain only serves HTML and plain JS. The libraries are loaded from github via CDN. GhostKat.org has never handles any of the file data in any way.

**Our website is showing the first 33 posts of the lower Plane, which requires ownership of 1 DBZ to post on.**
## Here is a tutorial for buying DBZ, and posting magnet links to our database!

1. First, add our [Our Kontract Address and ABI](https://github.com/GhostKatIII/GhostKat/blob/master/Contract_ABI) to your wallet
+ ![alt text](https://i.imgur.com/t8j4XyD.png "Adding GK")


2. From there you'll have access to buying DBZ at the price of *1 Ether for 1 DBZ. The ERC20 standard buy() function takes a msg.value of ether as an argument, and returnes the corresponding amount in dbz.*
+ ![alt text](https://i.imgur.com/bQOHPul.png "Buying Dubloonz")


3. After Buying Dubloonz you can post magnet links to the lower Plane!
+ ![alt text](https://i.imgur.com/ntOlJEI.png "Posting to lower PLane")
+ *There is one array on GhostKat that is free to post on! Just use function 'ridin' to post whatever you want, even gibberish posts!*
```C#
function Ridin (string postin) public  {
        MrB.push(postin);
       
}
```
Alternatively, [here](https://dontpanicsell.com/2017/11/18/dbz/) is an extended tutorial featuring Parity, for newbies to using smart contracts.

# 3: The Eternal Koin Offering (EKO)
There is one last step in the GhostKat Groove, and that is trust. We have to filter out the spam, the ads, and the bullshit posting that comes with the world wide web. To create our media haven with a healthy degree of trust, we will be giving away DBZ in phases to those who post popular content with honor and distinction. In the end, we will transfer ownership of the currency to the community, by running a transfer owner function on our contract.
```C#
contract owned {
    address public owner;

    function owned() public {
        owner = msg.sender;
    }

    modifier onlyOwner {
        require(msg.sender == owner);
        _;
    }

    function transferOwnership(address newOwner) onlyOwner public {
        owner = newOwner;
    }
}
```
That transfer will be to another contract; a virtual congress we call the **Dubloonz Piracy SyndiKat(DPS)**


That congress will be chosen by the Kommunity, using Dubloonz as voting shares.
[The Kommunity Kontract will use Ethereum standards set by the inventors themselves.](https://www.ethereum.org/dao#the-shareholder-association).


**The Dubloonz Piracy SyndiKat will be able to**
+ Withdraw funds raised through the purchase of DBZ
```C#
function eKo(uint256 amount) onlyOwner public {
    require(this.balance >= amount);
    msg.sender.transfer(amount);
}
```
+ Ban users from posting, and freeze DBZ assets
+ Mint DBZ
+ Set the public buy and sell price of DBZ
+ Most standard advanced features of ERC20

**Our roadmap is towards a completely decentralized autonomous syndikated peer 2 peer database**

Our GK Kontract has seven arrays.
+ Zero Palace - onlyOwner - zeroPost
+ Legend Palace - 99 DBZ - legendPost
+ Kat Kafe - 27 DBZ - katPost
+ Middle Palace - 5 DBZ - middlePost
+ Open Palace - 3 DBZ - openPost
+ Lower Plane -1 DBZ - lowerPost
+ Mr. Bones - 0 DBZ - ridin

*The numbers represent how much DBZ you must have in your cryptographic wallet to prove you are trusted enough to post on the array. Anyone can post to Mr.Bones, and we have an alternate interface targeting Mr.B on our Github. We do not wish to host this interface oursevles due to how unregulated it is.*

# PHASE I: The Eternal Charity of GhostKat
There are 3999 DBZ in existance. 999 are loaded into the contract itself, and can be purchased via the buy function. The rest is owned by ourselves, Chairmen Meow GhostKat III, the Super Lucky Kat, Royally, Plurally, Introducing. 

## We will be giving away 1,999 DBZ to users of GhostKat who add value to the system.
Once 1999 DBZ are out in the community, and the community is thriving, we will transfer ownership to the **DPS**. At the beginning, we are giving away only 1 DBZ at a time. **We will give 1 DBZ to anyone who sends us a magnet link they are seeding out at or above 500 mb/s.** Send us the magnet link via email at GhostKat2017@gmail.com, message us on Github, or just post that link to Mr.Bones. Be sure to include your ethereum address, and seed the magnet link via WebTorrent or WebTorrent compatible client.

# PHASE II: Open Fire
After phase I, we will give popular and effective users five Dubloonz, elevating them to middle post.From there we will stop giving DBZ to new people, and *anyone wishing to enter the community will need to buy DBZ.*


Fundraising is important, but secondary to establishing a trusted network of posters and hosters. After the community gets active and on its feet, we will give very large shares to the early adopters who are the most trusted. *We will continue giving away DBZ to the community until there are many Kats (27 DBZ), and a few Legend Kittens (99 DBZ).* At this point we will transfer ownership over to the Dubloonz Piracy SyndiKat. **If you don't trust us, all of our code is free to copy. What we do with fundraising money is completely transparent, and the lions share will be left for the DPS to distribute. The world needs piracy meow.** 

# PHASE III: Focus Fire
During this phase we will return our remaining DBZ balance of 1001 to the contract and the community. We will put all funds raised towards establishing an expanded GK network that handles music, TV, and Movies. By divesting, we will have no legal or literal connection to DBZ, but this is better so that the system is completely distributed through the community. We hope to again reward members of the community in all aspects, in DBZ, and by showing our good faith by also giving over most DBZ raised before transfer.


## All we need to do is connect to one another
It is time to establish a new protocol that allows for the free and easy transfer of information between peers. We humbly put forth GhostKat as a method, a style, and a protocol if you'd like. It is easy to repurpose this method to act like the greater internet, with websites and social media all being hosted peer 2 peer.

**If you are out for glory, booty, join the Dubloonz Piracy SyndiKat for free by contributing!**

**1 DBZ to anyone who sends us a magnet link they are seeding out at or above 500 mb/s.** Send us the magnet link via email at GhostKat2017@gmail.com, message us on Github, or just post that link to Mr.Bones. Be sure to include your ethereum address, and seed the magnet link via WebTorrent or WebTorrent compatible client.

**5 DBZ to the first person to get our interface running on firefox and mobile browsers!**
We have an issue open on our github, so you can comment there, or send us your solution directly at GhostKat2017@gmail.com. Web3 js appears to crash easily.



![alt text](https://webtorrent.io/img/WebTorrent.png "WebTorrent")

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/ETHEREUM-YOUTUBE-PROFILE-PIC.png/240px-ETHEREUM-YOUTUBE-PROFILE-PIC.png "Ethereum")

![alt text](http://website-thumbnails.informer.com/thumbnails/280x202/i/infura.io.png "INFURA")

