const Discord = require('discord.js');
const bot = new Discord.Client();

const PREFIX = 'B!';

var version = '1.0.1';

bot.on('ready', () => {
    console.log('This bot is online!');
    bot.user.setActivity('Watching B!Help');
})

bot.on('message', msg=>{
    if(msg.content === "B!Hello"){
        msg.reply('Hello I Am A BroBot, How Is your Day Going :bust_in_silhouette:');
    }    
})

bot.on('message', msg=>{
    if(msg.content === "B!Help"){
        msg.reply(':bust_in_silhouette: HELP PAGE : Use B!Hello or B!Help For This Help Page : More Features Comming Soon..');
    }    
})

bot.on('guildMemberAdd', member => {
    let channel = member.guild.channels.find('name', 'welcome');
    let memberavatar = member.user.avatarURL
        if (!channel) return;
        let embed = new Discord.RichEmbed()
        .setColor('RANDOM')
        .setThumbnail(memberavatar)
        .addField(':bust_in_silhouette: | name : ', `${member}`)
        .addField(':microphone2: | Welcome!', `Welcome to the server, ${member}`)
        .addField(':id: | User :', "**[" + `${member.id}` + "]**")
        .addField(':family_mwgb: | Your are the member', `${member.guild.memberCount}`)
        .addField("Name", `<@` + `${member.id}` + `>`, true)
        .addField('Server', `${member.guild.name}`, true )
        .setFooter(`**${member.guild.name}**`)
        .setTimestamp()

        channel.sendEmbed(embed);
});

bot.on('guildMemberAdd', member => {

    console.log(`${member}`, "has joined" + `${member.guild.name}`)
});

const token = process.env.TOKEN;
client.login(process.env.BOT_TOKEN);
