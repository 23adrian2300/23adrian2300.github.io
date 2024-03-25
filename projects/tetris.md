---
layout: project
type: project
image: img/tetris/tetris.png
title: "Tetris"
best: 6
date: 2023
published: true
labels:
  - C++
  - SFML
  - Github
summary: "SMFL Project for C++ Classes"
---

## Description
Tetris is a final project for the 'Programming in C++' course. It was written with the help of the SFML library, which enables graphics and game creation. It also allows handling various types of events.

Source: <a href="https://github.com/23adrian2300/CPP_projekt-AGH">AGH/CPP_projekt/Tetris</a>

SFML's Graphics module, encapsulated in Graphics.hpp, simplifies 2D graphics rendering across platforms, offering efficient rendering of sprites, textures, and primitives. With hardware acceleration support, it ensures smooth performance, while its intuitive API facilitates resource management for cleaner code. This versatility makes it ideal for various applications, from games to multimedia presentations.

## App appearance

<div class="text-center p-4">
  <img height="300" src="../img/tetris/tetrisGame.png" class="img-thumbnail" >
</div>

It was also my first major project in C++. However, it wasn't very difficult due to the learning process in previous labs, the solutions of which can be found at the following link:
<a href="https://github.com/23adrian2300/CPP-AGH">AGH/CppProgramming</a>

An example of event handling code looks like this:

```cpp
void Game::handleEvents()
{
    float time = clock.getElapsedTime().asSeconds();
    clock.restart();
    timer += time;
    auto event = make_shared<sf::Event>();
    while (window->pollEvent(*event))
    {
        if (event->type == sf::Event::Closed)
        {
            window->close();
        }

        if (event->type == sf::Event::KeyPressed)
        {
            switch (event->key.code)
            {
            case sf::Keyboard::Up:
                change = true;
                break;
            case sf::Keyboard::Right:
                ++directionX;
                break;
            case sf::Keyboard::Left:
                --directionX;
                break;
            default:
                break;
            }
        }
    }

    if (sf::Keyboard::isKeyPressed(sf::Keyboard::Down))
    {
        delay = 0.03;
    }
}
```
## Small rework of the project
Recently, I decided to improve this project a bit. I added .h files and, above all, CMakeLists.txt files. Thanks to them, it's easy to compile the code in different environments. I prepared two variants, one is for Visual Studio and the other for CLion. They automatically download the required SFML library, eliminating the need to go through the installation process. Furthermore, I made some improvements to the code itself to better conform to prevailing standards.

