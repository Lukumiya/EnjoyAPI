# EnjoyAPI

Ассинхронный клиент для API EnjoyMickeyBot

Установка:

    

Пример:

```py
from EnjoyAPI.EnjoyAPI import EnjoyAPI


from discord.ext import commands

bot = commands.Bot(command_prefix='>>')

enjoyClient = EnjoyAPI(bot, 'ваш токен тут')
@bot.command()
async def checkUser(ctx: commands.Context, userID: int):
    data = await enjoyClient.check(userID)
    await ctx.send(f'Вот данные от пользователя с ID, ```{data}```')


bot.run('тут токен бота')
```





Ключ не давали, не тестил, если будут проблемы/вопросы [Issues](https://github.com/KotypeyPyEdition/EnjoyAPI/issues)