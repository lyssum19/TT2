using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;
using TTT2;

namespace TTT2
{
    public partial class Form1 : Form
    {
        protected string b1, b2, b3, b4, b5, b6, b7, b8, b9;
        public Form1()
        {
            InitializeComponent();
        }

        bool isPlayerX = true;

        private void Form1_Load(object sender, EventArgs e)
        {

        }

      

        private void button1_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button1.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button1.Text = "O";
                isPlayerX = true;
            }
            b1 = button1.Text;
            button1.Enabled = false;
            label3.Text = declareWin();
        }

        private void button2_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button2.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button2.Text = "O";
                isPlayerX = true;
            }
            b2 = button2.Text;
            button2.Enabled = false;
            label3.Text = declareWin();
        }

        private void button10_Click(object sender, EventArgs e)
        {
            button1.Text = string.Empty;
            button2.Text = string.Empty;
            button3.Text = string.Empty;
            button4.Text = string.Empty;
            button5.Text = string.Empty;
            button6.Text = string.Empty;
            button7.Text = string.Empty;
            button8.Text = string.Empty;
            button9.Text = string.Empty;
            button1.Enabled = true;
            button2.Enabled=true;
            button3.Enabled=true;
            button4.Enabled=true;
            button5.Enabled=true;
            button6.Enabled=true;
            button7.Enabled=true;
            button8.Enabled=true;
            button9.Enabled=true;
        }

        private void button11_Click(object sender, EventArgs e)
        {
            MessageBox.Show("Exit Game", "TicTacToe", MessageBoxButtons.OK, MessageBoxIcon.Information);
            this.Close();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button3.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button3.Text = "O";
                isPlayerX = true;
            }
            b3 = button3.Text;
            button3.Enabled = false;
            label3.Text = declareWin();
        }

        private void button4_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button4.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button4.Text = "O";
                isPlayerX = true;
            }
            b4 = button4.Text;
            button4.Enabled = false;
            label3.Text = declareWin();
        }

        private void button5_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button5.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button5.Text = "O";
                isPlayerX = true;
            }
            b5 = button5.Text;
              button5.Enabled = false;
            label3.Text = declareWin();
        }

        private void button6_Click(object sender, EventArgs e)
        {
             if (isPlayerX)
            {
                button6.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button6.Text = "O";
                isPlayerX = true;
            }
             b6 = button6.Text;
              button6.Enabled = false;
            label3.Text = declareWin();
        }

        private void button7_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button7.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button7.Text = "O";
                isPlayerX = true;
            }
            b7 = button7.Text;
            button7.Enabled = false;
            label3.Text = declareWin();
        }

        private void button8_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button8.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button8.Text = "O";
                isPlayerX = true;
            }
                b8 = button8.Text;
            button8.Enabled = false;
            label3.Text = declareWin();
        }

        private void button9_Click(object sender, EventArgs e)
        {
            if (isPlayerX)
            {
                button9.Text = "X";
                isPlayerX = false;
            }
            else
            {
                button9.Text = "O";
                isPlayerX = true;
            }
            b9 = button9.Text;
            button9.Enabled = false;

            label3.Text = declareWin();
        }


        
        public string declareWin()
        {
            if (b1 == b2 && b2 == b3)
            {
                return $"Player {b1} Wins!";
            }
            else if (b1 == b4 && b4 == b7)
            {
                return $"Player {b1} Wins!";
            }
            else if (b1 == b5 && b5 == b9)
            {
                return $"Player {b1} Wins!";
            }
            else if (b4 == b5 && b5 == b6)
            {
                return $"Player {b4} Wins!";
            }
            else if (b7 == b8 && b8 == b9)
            {
                return $"Player {b7} Wins!";
            }
            else if (b2 == b5 && b5 == b8)
            {
                return $"Player {b2} Wins!";
            }
            else if (b3 == b6 && b6 == b9)
            {
                return $"Player {b3} Wins!";
            }
            else if (b3 == b5 && b5 == b7)
            {
                return $"Player {b3} Wins!";
            }
            else
            {
                return "";
            }
        }
    }
}
