# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[HRÁT!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Takže než začneme, jak by jsi chtěl číst?

`publish("show_options_bottom")`

# intro-start-2

n3: A teď začněme náš příběh...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: TOTO JE ČLOVĚK

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: A TOTO JE LIDSKÁ ÚZKOST

n: _TY_ JSI ÚZKOST

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ne. Ne, ne, neposlouchám. Zkontroluji telefon.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TVÝM ÚKOLEM JE CHRÁNIT SVÉHO ČLOVĚKA PŘED *NEBEZPEČÍM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ach! Projíždíte svůj život na Twitteru! Znovu!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Jo, říkám si, proč si prostě nesednu a neposlouchám své myšlenky častěji.

`hong({eyes:"neutral"});`

n: RYCHLE, VARUJTE JE PŘED *NEBEZPEČÍM!*

```
bb({eyes:"look"});
```

[Ale ne, podívej se na tu hroznou zprávu!](#act1d_news)

[Ale ne, je ten tweet tajně o *nás*?](#act1d_subtweet)

[Hej, GIF kočky pijící mléko](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: To je roztomilé, já...

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KOČKY NEUMÍ TRÁVIT MLÉKO A MY JSME HROZNÍ LIDÉ, PROTOŽE SE NÁM LÍBÍ TÝRÁNÍ ZVÍŘAT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



