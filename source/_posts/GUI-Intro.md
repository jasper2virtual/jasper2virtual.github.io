---
title: GUI Intro
tags:
  - Java
  - learning journal
date: 2021-07-20 23:30:10
---
Learn from 
{% link Bro Code video https://www.youtube.com/watch?v=xk4_1vDrzzo&t=2953s %} 

Try to using desktop dialog box to get keyboard input, and show the result too.  

{% codeblock lang:java %}
import javax.swing.JOptionPane;

public class Hello {
	public static void main(String[] args) {
		String name = JOptionPane.showInputDialog("What is your Name?");
		int age = Integer.parseInt(JOptionPane.showInputDialog("How old are you?"));
		double height = Double.parseDouble(JOptionPane.showInputDialog("How tall are you?"));
		JOptionPane.showMessageDialog(null,
				String.format("Your name is %s.\nYou are %d years old.\nYour height is %.2f cm.", name, age, height));
	}
}
{% endcodeblock %}