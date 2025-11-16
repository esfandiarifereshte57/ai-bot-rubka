from rubka import Robot
from rubka.context import Message
import requests

bot = Robot("EBGJJ0NBFYOAYWKGFYJEVXMEIXNOJRACGBVITISMHIOFSFCIOYYYXWHSUCPBQGCG")

@bot.on_message()
def handle_message(bot: Robot, message: Message):
    if not message.text:
        return

    text = message.text.strip()
    low_text = text.lower()

    if low_text == "/start":
        message.reply("سلام 👋\nمن هوش مصنوعی هستم 🤖\nهر متنی برام بفرستی، با هوش مصنوعی پاسخ میدم 💬")
        return

    if "خوبی" in low_text:
        message.reply("خوبم ممنون! شما چطور؟ 😊")
        return
    elif "چطوری" in low_text:
        message.reply("خوبم مرسی! چه خبر؟")
        return
    elif "سلام" in low_text:
        message.reply("سلامت باشی! 😊")
        return

    message.reply("🤔 در حال فکر کردن...")

    try:
        response = requests.get(
            "https://hoshi-app.ir/api/chat-gpt.php",
            params={"text": text, "lang": "fa"},
            timeout=10
        )
        if response.status_code == 200:
            data = response.json()
            result = data.get("result") or data.get("Result")
            reply_text = result if result else "❌ پاسخی دریافت نشد"
        else:
            reply_text = "⚠️ خطا در ارتباط با سرور"
    except Exception:
        reply_text = "⚠️ خطا در ارتباط با سرور"

    message.reply(reply_text)

bot.run()
