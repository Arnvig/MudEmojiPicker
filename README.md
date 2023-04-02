# MudEmojiPicker

For some reason MudDialog do not work, the rest works...

It use Mudblazor, Twemoji.

The code is mainly copy from a bigger project
https://github.com/Faellesskabet/kuliv.dk


Remember to add 
`builder.Services.AddSingleton<EmojiService>();`
And we have two different ways to get the emojis
` <MudIcon Icon="@EmojiService.GetSvgValue("🤣")"/> `

If you use the Twemoji.E1f0cf be aware some of the "Null" space there is in emoji is delete.
` <MudIcon Icon="@Twemoji.E1f0cf"/>  `

Value as a string. 
` <MudEmojiPicker @bind-Value="context.Emoji"/>`
