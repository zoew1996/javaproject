# javaproject
package Image;

import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

import javax.swing.JButton;
import javax.swing.JComboBox;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JList;
import javax.swing.JPanel;
import javax.swing.JScrollPane;
import javax.swing.JTextArea;

public class project extends JFrame implements ActionListener {
	//public 
	JPanel p = new JPanel();
	JList list = new JList();
	JLabel rtype = new JLabel("Type of Room");
	String[] room = new String[] {"Davy Jones' Locker", "Crow's Nest", "Caption Jack Sparrow"};
	String[] extra = new String[] {"Ocean View", "Locked Inside", "Small Window"}; 
	
	//iceburg 
	//lifejackets
	JComboBox jc = new JComboBox(extra);
	//Object selected = roombox.getSelectedItem();	
	JComboBox roombox = new JComboBox(room);
	JButton cash = new JButton ("Cash");
	JButton credit = new JButton ("Credit");
	JButton check = new JButton ("Check");
	JButton b1 = new JButton("Complete");
	JButton b2 = new JButton("Add Discount");
	JButton b3 = new JButton("Print");
	Double total; 	

	
	public static void main(String[] args) { 
		project app =  new project();
		app.setSize(600,600);
		app.setDefaultCloseOperation(EXIT_ON_CLOSE);
		app.setTitle("Titantic 2 Shops");
		app.setVisible(true);
		
	}

	//Constructor Method 
	project(){
		p.setSize(600,600);
		p.add(b1);
		p.add(b2);
		p.add(b3);
		p.add(credit);
		p.add(cash);
		p.add(check);
		p.add(rtype);
		p.add(roombox);
		p.add(jc);
		p.add(list);
		roombox.addActionListener(this);
		//box.setBounds();
		b1.addActionListener(this);
		b2.addActionListener(this);
		b3.addActionListener(this);
		credit.addActionListener(this);
		check.addActionListener(this);
		cash.addActionListener(this);
		
		add(p);
	}
	
	@Override
	//"Davy Jones' Locker", "Crow's Nest", "Caption Jack Sparrow"
	public void actionPerformed(ActionEvent arg0) {

	
	}

}
