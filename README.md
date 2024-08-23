<h1 align="center">DukDuke JAVA GUI Development Kit</h1>


DukDuke JAVA GUI Development Kit is a comprehensive toolset designed to simplify and accelerate the process of developing Java-based user interfaces. This library helps developers create effective and modern graphical user interfaces in Java. DukDuke facilitates rapid prototyping and development processes with its extensible and customizable components, aiming to enhance productivity in application development

## Usage
### Requirements

- **Java Development Kit (JDK) 17 or above**  
  **Recommended version:** OpenJDK 22.0
- **Gradle is recommended.**

### How to Import Templates and Example Variables?
- If you want to use predefined variables, there are a few things you need to know. First, you should learn how to import these variables into your project. Each predefined variable's file usually has an informative section at the top (if available). This section provides recommendations, important details, and instructions on how to use the variable. Additionally, predefined variables often include a few guide sections. For example, like this: 
    ```java
    import javax.swing.*;
    import java.awt.*;
    import java.awt.event.ActionEvent;
    import java.awt.event.ActionListener;
    import java.awt.event.MouseAdapter;
    import java.awt.event.MouseEvent;

	JButton closeButton = new JButton("X");
        closeButton.setForeground(new Color(r_value, g_value, b_value)); //The color of the “X” on this button [Recommended color: 255, 255, 255]
        closeButton.setBackground(new Color(r_value, g_value, b_value)); //Normal color of this button [Recommended color: 41, 41, 41]
        closeButton.setBorder(BorderFactory.createEmptyBorder());
        closeButton.setFocusPainted(false);
        closeButton.setContentAreaFilled(false);
        closeButton.setOpaque(true);
        closeButton.setBounds(x_pos, y_pos, width, height); //Size and location of this button [Recommended size: 32, 25]
        closeButton.setFont(new Font("Font", Font.TYPE, size)); //The size, font and type of this “X” [Recommended size, font and type: Segoe UI, PLAIN, 11
        closeButton.setHorizontalAlignment(SwingConstants.CENTER);
        closeButton.addMouseListener(new MouseAdapter() {
            @Override
            public void mouseEntered(MouseEvent e) {
                closeButton.setBackground(new Color(r_value, g_value, b_value)); //The color of this button with the cursor on it [Recommended color: 233, 50, 50]
            }
            @Override
            public void mouseExited(MouseEvent e) {
                closeButton.setBackground(new Color(r_value, g_value, b_value)); //This is the normal color of the button, but the color after the cursor passes over it, not the initial color [Recommended color: 41, 41, 41]
            }
        });

        closeButton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
            	System.exit(0);
            }
        });
As you can see, there are guide sections in some lines. Now, let's move on to how to use these predefined variables. If you import these variables directly into your project without any modifications, you'll encounter errors. First, you need to fill in the sections indicated in the guide and import the necessary libraries. All the required libraries can be found in the predefined variable templates. Additionally, the other sections that need to be filled out (if available) are as follows:

- `r_value` = The value of the red color
- `g_value` = The value of the green color
- `b_value` = The value of the blue color

Aside from these, if applicable:

- `x_pos` = The horizontal position of the variable
- `y_pos` = The vertical position of the variable
- `width` = The width of the variable
- `height` = The height of the variable

These values must be filled in. Additionally, if the variable is a text or contains text, the following fields should also be filled out:

- `size` = The size of the text
- `"Font"` = The font of the text
- `TYPE` = The type of the text (e.g., **Bold**, *Italic*, Plain)

### How to use templates?
- If you want to use ready-made templates, there are a few things you need to know. The JDK version of the templates should always be Oracle OpenJDK 22.0.2 or higher. It is also recommended to open these templates with [IntelliJ IDEA](https://www.jetbrains.com/idea/)

## Licensing
This project is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). 

If you use **ANY** code from the source:
- You must disclose the source code of your modified work and the source code you took from this project. This means you are not allowed to use code from this project (even partially) in a closed-source and/or obfuscated application.
- You must state clearly and obviously to all end users that you are using code from this project.
- Your application must also be licensed under the same license.
 
## Contact

For questions, feedback, or suggestions, please contact us using the following methods:

- **Email:** [*official0xdevelopment@outlook.com*]()
- **Discord:** [*0x87926*]()
