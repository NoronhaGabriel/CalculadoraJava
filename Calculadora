package Projeto;

import java.awt.EventQueue;
import javax.swing.JFrame;
import javax.swing.JTextField;
import javax.swing.JButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;


public class Calculadora extends JFrame {

	private JFrame frame;
	private JTextField textField;
	private double num1, num2, result;
	private String operation;

	public static void main(String[] args) {
		EventQueue.invokeLater(() -> {
			try {
				Calculadora window = new Calculadora();
				window.frame.setVisible(true);
			} catch (Exception e) {
				e.printStackTrace();
			}
		});
	}

	public Calculadora() {
		initialize();
	}

	private void initialize() {
		frame = new JFrame();
		frame.setTitle("Calculadora");
		frame.setBounds(100, 100, 300, 400);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.getContentPane().setLayout(null);

		textField = new JTextField();
		textField.setBounds(10, 11, 260, 40);
		frame.getContentPane().add(textField);
		textField.setColumns(10);

	
		JButton btn1 = new JButton("1");
		btn1.setBounds(10, 62, 60, 40);
		btn1.addActionListener(e -> textField.setText(textField.getText() + "1"));
		frame.getContentPane().add(btn1);

		JButton btn2 = new JButton("2");
		btn2.setBounds(80, 62, 60, 40);
		btn2.addActionListener(e -> textField.setText(textField.getText() + "2"));
		frame.getContentPane().add(btn2);

		JButton btn3 = new JButton("3");
		btn3.setBounds(150, 62, 60, 40);
		btn3.addActionListener(e -> textField.setText(textField.getText() + "3"));
		frame.getContentPane().add(btn3);

		JButton btnAdd = new JButton("+");
		btnAdd.setBounds(220, 62, 50, 40);
		btnAdd.addActionListener(e -> {
			num1 = Double.parseDouble(textField.getText());
			operation = "+";
			textField.setText("");
		});
		frame.getContentPane().add(btnAdd);

		JButton btn4 = new JButton("4");
		btn4.setBounds(10, 113, 60, 40);
		btn4.addActionListener(e -> textField.setText(textField.getText() + "4"));
		frame.getContentPane().add(btn4);

		JButton btn5 = new JButton("5");
		btn5.setBounds(80, 113, 60, 40);
		btn5.addActionListener(e -> textField.setText(textField.getText() + "5"));
		frame.getContentPane().add(btn5);

		JButton btn6 = new JButton("6");
		btn6.setBounds(150, 113, 60, 40);
		btn6.addActionListener(e -> textField.setText(textField.getText() + "6"));
		frame.getContentPane().add(btn6);

		JButton btnSub = new JButton("-");
		btnSub.setBounds(220, 113, 50, 40);
		btnSub.addActionListener(e -> {
			num1 = Double.parseDouble(textField.getText());
			operation = "-";
			textField.setText("");
		});
		frame.getContentPane().add(btnSub);

		JButton btn7 = new JButton("7");
		btn7.setBounds(10, 164, 60, 40);
		btn7.addActionListener(e -> textField.setText(textField.getText() + "7"));
		frame.getContentPane().add(btn7);

		JButton btn8 = new JButton("8");
		btn8.setBounds(80, 164, 60, 40);
		btn8.addActionListener(e -> textField.setText(textField.getText() + "8"));
		frame.getContentPane().add(btn8);

		JButton btn9 = new JButton("9");
		btn9.setBounds(150, 164, 60, 40);
		btn9.addActionListener(e -> textField.setText(textField.getText() + "9"));
		frame.getContentPane().add(btn9);

		JButton btnMul = new JButton("*");
		btnMul.setBounds(220, 164, 50, 40);
		btnMul.addActionListener(e -> {
			num1 = Double.parseDouble(textField.getText());
			operation = "*";
			textField.setText("");
		});
		frame.getContentPane().add(btnMul);

		JButton btn0 = new JButton("0");
		btn0.setBounds(10, 215, 60, 40);
		btn0.addActionListener(e -> textField.setText(textField.getText() + "0"));
		frame.getContentPane().add(btn0);

		JButton btnClear = new JButton("C");
		btnClear.setBounds(80, 215, 60, 40);
		btnClear.addActionListener(e -> textField.setText(""));
		frame.getContentPane().add(btnClear);

		JButton btnEqual = new JButton("=");
		btnEqual.setBounds(150, 215, 60, 40);
		btnEqual.addActionListener(e -> {
			num2 = Double.parseDouble(textField.getText());
			switch (operation) {
				case "+": result = num1 + num2; break;
				case "-": result = num1 - num2; break;
				case "*": result = num1 * num2; break;
				case "/": result = num1 / num2; break;
			}
			textField.setText(String.valueOf(result));
		});
		frame.getContentPane().add(btnEqual);

		JButton btnDiv = new JButton("/");
		btnDiv.setBounds(220, 215, 50, 40);
		btnDiv.addActionListener(e -> {
			num1 = Double.parseDouble(textField.getText());
			operation = "/";
			textField.setText("");
		});
		frame.getContentPane().add(btnDiv);
	}
}
