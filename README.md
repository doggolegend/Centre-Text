# Centre-Text
How to centre text in sfml 3


```cpp
// How to centre (center) text in sfml 3
sf::Text text(poppins);
text.setString("Press 1 to begin!");
text.setCharacterSize(24);
text.setFillColor(sf::Color::Black);
text.setStyle(sf::Text::Bold);
// Centre below
text.setOrigin({ text.getScale().x + text.getString().getSize() * (text.getLetterSpacing() + text.getCharacterSize() / 2.f) / 2.f, text.getScale().y });
text.setPosition({ windowSize.x / 2.f, windowSize.y / 2.f});

// Then you can draw it!
```
