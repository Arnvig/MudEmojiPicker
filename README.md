# MudEmojiPicker

For some reason do it not work.

It use Mudblazor, Twemoji.

It is implamentet on a bigger project and working
https://github.com/Faellesskabet/kuliv.dk

Remember to add 
`builder.Services.AddSingleton<EmojiService>();`
And we have two different ways to get the emojis
` <MudIcon Icon="@EmojiService.GetSvgValue("🤣")"/> `

If you use the Twemoji.E1f0cf be aware some of the "Null" space there is in emoji is delete.
` <MudIcon Icon="@Twemoji.E1f0cf"/>  `

Value as a string. 
` <MudEmojiPicker @bind-Value="context.Emoji"/>`
