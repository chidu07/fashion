import javax.swing.*;  
import java.awt.event.*;
import java.awt.Color;
public class demoswing1 {  
public static void main(String[] args) {  
JFrame f=new JFrame();//creating instance of JFrame 
 
 final JTextField tf=new JTextField(); 
 tf.setBounds(50,100,95,20);         
JButton b1=new JButton("add");//creating instance of JButton  
b1.setBounds(150,100,100, 40);//x axis, y axis, width, height  
b1.setBackground(Color.GREEN);
b1.setForeground(Color.BLACK);
          
//adding button in JFrame  
          
JButton b2=new JButton("update");//creating instance of JButton  
b2.setBounds(230,100,120, 40);//x axis, y axis, width, height  
b2.setBackground(Color.RED);
b2.setForeground(Color.BLACK);
                   


b1.addActionListener(new ActionListener ()  {
public void actionPerformed(ActionEvent e)
{
    tf.setText("add");
    }
});

b2.addActionListener(new ActionListener ()  {
public void actionPerformed(ActionEvent e)
{
    tf.setText("update");
    }
});

f.add(b1);
f.add(b2);
f.add(tf);
f.getContentPane().setBackground(Color.gray);
f.setSize(400,500);//400 width and 500 height  
f.setLayout(null);//using no layout managers  
f.setVisible(true);//making the frame visible  
}  
}
