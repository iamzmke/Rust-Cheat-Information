<a href="Ω"><img src="http://readme-typing-svg.herokuapp.com?font=VT323&size=90&duration=2000&pause=1000&color=F70000&center=true&random=false&width=1100&height=140&lines=%E2%98%A6+Rust+Information+%E2%98%A6;%E2%98%A6+By+Smoke+%E2%98%A6" alt="Ω" /></a>

After the best part of 5 years providing and developing cheats for private consumers we've gained a large amount of knowledge on features, exploits and general security practises within the game Rust, So im creating this repository to document knowledge
and information on said topics.

## Cerberus

#### What is it?
Cerberus is a heuristic & rules based engine used to flag and in most cases temporarily ban suspected cheaters, Developed by East Anti Cheat and supported with data by Facepunch Studios.

#### How does it work?
No one outside of Facepunch & EAC knows 100%, Though we've experimented ALOT over the years. There is also ALOT of miss information online on forums such as unknowncheats and other forums alike, But it boils down to this. Facepunch gathers a whole lot of statistics on every player, Who you hit, who you kill, how far you run, how many items you've placed, who you revive, how much you build, where you projectiles hit, where your projectiles are shot from, your hours, your hardware and literally every single thing that happens within the game. They then take all the data from all players bad and good, and create a score to determine whether you are cheating. When a player reports you if your score is over a certain threshold you get a temporary 3 day ban onthe account. Without a report the system does not automatically ban anyone, That being said you can still be manually banned by a developer when your score gets too high. Cerberus does not permanently ban anyone for the first ban.

#### How can you tell a manual ban from a cerberus ban?
Facepunch moderators will usually visibly come to you, or atleast connect to your server before they ban you or they will spawn rockets on top of you before banning you, a temporary ban from a moderator/admin are almost always 5-7 days long if they arent 100% sure, if they are 100% sure you are cheating they will instantly permanently game ban you. Ceberus bans will come soon after a player reports you (typically within 45 seconds of a report), if your heuristic score is very high you will instantly get a 3 day ban, when playing on that account again you will be permanently banned upon a second instance of players reporting you, if your bypass/cheat is detected but has a very low amount of users and your heuristic score is below the cheater threshold you can get up to 5 3 day bans before the permanent ban is issued, typically issued by a game developer as after 5 bans the account is raised within the facepunch admin panel for manual review. if you make the mistake of contacting the facepunch developers over discord you risk getting your account instantly permanently banned.

#### Why shouldnt i contact a Facepunch admin and try to get unbanned?
Facepunch admins have been publicly known to join discords related to cheating and cheater communities to log the accounts within the servers, amoung many many community driven projects made to detect cheaters within discords and flag their accounts to community server moderators. There are many bots around that flag guilds that discord accounts are a part of to aid admins and moderators of rust servers in detecting potential cheaters and scripters through their community ties. So it is always recommended to use an alt to contact admins or to use an alt in the cheating scene in general under a seperate alias.

#### Why is any of this relevant?
Throughout this document i will be refering to cerberus scores to indicate the chances of these features flagging the user account, I will format it as (CS: flagChance) for booleans and (CS: flagChance * value) for floating points and integers


## Projectile Modifications

| Path | Max Values     | Description                |
| :-------- | :------- | :------------------------- |
| `Projectile->thickness` | `0.01f - 1.0f` | Gives the effect of expanding the targets hitbox |
