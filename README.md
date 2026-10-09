# CGMidterm

Part 2: I used a Fresnel effect to create the appearance of a shiny object. 
        I used this because I couldn't remember how to do the lighting shown in class and this had an effect that would simulate having a reflective object
        To make the shader I made a base texture and then added a Fresnel effect with it.
        

Part 3: For the waterfall shader I used a float velocity variable with a value of -0.5 and multiplied it by time,
        I then used a tiling and offset node to make the object scroll at an offset
        I then used the split node to only scroll on the Y axis to get the waterfall affect
        I went about it this way because waterfalls fall down and if you don't use the split function then the offset will be in all directions

Part 4: For the taking damage shader I started with creating 2 color nodes, 2 texture nodes, and a float node
        using the 2 colour nodes a multiplied them with UVs to make 2 different colours.
        I then put each node into their own colour
        On one of the nodes I used another split function to get only the transparency value of the shader.
        I then added a float value with the transparent from the split function to then multiply with the other texture to create an effect when taking damage.
        The float value has a slider that can change based on when the player takes damage.
        The Damage colour will not always be seen so it should only appear when the player takes damage. 
        By making one shader transparent the character will appear to not be taking damage all the time until they take damage
