# csharpCalculator

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Calculator
{
    public partial class Form1 : Form
    {

        int value1, value2;
        char sign;

        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "1";
        }

        private void button2_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "2";
        }

        private void button3_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "3";
        }

        private void button5_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "4";
        }

        private void button6_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "5";
        }

        private void button7_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "6";
        }

        private void button8_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "7";
        }

        private void button9_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "8";
        }

        private void button10_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "9";
        }

        private void button11_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = richTextBox2.Text + "0";
        }

        private void button4_Click(object sender, EventArgs e)
        {
            richTextBox2.Text = "";
        }

        private void button13_Click(object sender, EventArgs e)
        {
            value1 = int.Parse(richTextBox2.Text);
            sign = '-';
            richTextBox2.Text = "";
        }

        private void button14_Click(object sender, EventArgs e)
        {
            value1 = int.Parse(richTextBox2.Text);
            sign = '/';
            richTextBox2.Text = "";
        }

        private void button15_Click(object sender, EventArgs e)
        {
            value1 = int.Parse(richTextBox2.Text);
            sign = '*';
            richTextBox2.Text = "";
        }

        private void button16_Click(object sender, EventArgs e)
        {
            value2 = int.Parse(richTextBox2.Text);
            int result;
            if(sign == '+') {
                result = value1 + value2;
                richTextBox2.Text = result.ToString();
            }

            if (sign == '-')
            {
                result = value1 - value2;
                richTextBox2.Text = result.ToString();
            }
            
            if (sign == '*')
            {
                result = value1 * value2;
                richTextBox2.Text = result.ToString();
            }

            if (sign == '/')
            {
                result = value1 / value2;
                richTextBox2.Text = result.ToString();
            }
        }

        private void button12_Click(object sender, EventArgs e)
        {
            value1 = int.Parse(richTextBox2.Text);
            sign = '+';
            richTextBox2.Text = "";
        }
    }
}

# csharpCalculator Image

![image](https://user-images.githubusercontent.com/106742344/216639594-487a6d9f-dd16-4ba2-9887-ec6eaab8c7a3.png)
