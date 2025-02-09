import random


def generate_message(name):
    name = name.lower()

    if name == "celalet":
        poem = f"""### Cəlalət

Cəlalət, gözəlliyin adı,  
Sözlərdə canlanır, ruhda yanar.  
Gecə ulduzları, parlayan işıq,  
Səninlə dolur, hər an, hər an.

Sözlərin bir nağıl, dodaqlarda dans,  
Hər bir kəlmə, bir sevda, bir şans.  
Yürekdə açılan, çiçəklər kimi,  
Cəlalət, sən bir bahar, bir sevgi.

Gözlərin dəniz, dərin və mavi,  
Hər dalğa bir xatirə, bir həsrət.  
Sənə yazdım, bu sevda şeirini,  
Cəlalət, sən mənim ilham pərim."""
        return poem.strip()

    elif name == "elnurə":
        poem = f"""
        ### Elnurə

Elnurə, adınla başlar gün,  
Səninlə dolur, hər an, hər gün.  
Gözlərin nur saçan, sevgi dolu,  
Sənin sayəndə, dünya bir yurd olur.

Ana, əllərin şəfqət dolu,  
Hər bir öpüşün, bir sevda, bir qolu.  
Sözlərin nağıl, ruhumda yankı,  
Elnurə, sən mənim həyatımın anka.

Hər çiçək açar, sənin üçün,  
Sevgin, mənim gücüm, bir ömür boyu.  
Yürekdə daima, sevgi və səs,  
Elnurə, sən mənim ən gözəl hissəm.  
        """
        return poem.strip()

    elif name == "şükufə":
        poem = f"""
        ### Şükufə

Şükufə, adınla açar bahar,  
Gözlərin parıldar, sevda dolu yar.  
Hər gül açıldığında, sən gülümsərsən,  
Sözlərin bir nağıl, ruhuma sığar.

Sənin sevgin, bir dəniz, dərin və mavi,  
Hər dalğa bir həsrət, bir xatirə, canlı.  
Ürəyimdə çiçəklər açar, sənlə,  
Şükufə, səninlə dolur hər bir gün.

Gözlərindəki nur, gecəni aydınlatar,  
Sənin sayəndə, dünya bir cənnət olar.  
Hər anımda varsan, sən mənim ilham,  
Şükufə, sən mənim həyatımın ən gözəl sədası..  
        """
        return poem.strip()

    messages = [
        f"Əziz {name.capitalize()}, zəhmətin, sevgin və gücün dünyanı daha gözəl edir. Dünya Qadınlar Günün mübarək! 💐",
        f"{name.capitalize()}, sənin kimi güclü və zərif qadınlar sayəsində dünya daha gözəl yerdir. Bu gün və hər gün çox dəyərlisən! 🌸",
        f"{name.capitalize()}, həyatın hər sahəsində işıq saçan, ilham verən qadınlardan biri olaraq səni sevgi ilə salamlayırıq. Qadınlar Günün mübarək! 💖",
        f"Güclü, cəsur və sevgi dolu qadınların günü mübarək olsun! {name.capitalize()}, sənin varlığın dünyaya gözəllik qatır. 🌹",
        f"{name.capitalize()}, sənin kimi ilham verən qadınlar sayəsində dünya daha güclüdür! Bu gün və hər gün dəyərli olduğunu unutma. Kadınlar Günün mübarək! ✨"
    ]

    return random.choice(messages)


if __name__ == "__main__":
    name = input("Zəhmət olmasa adınızı daxil edin: ")
    message = generate_message(name)
    print("\nSizin üçün mesaj:\n")
    print(message)
