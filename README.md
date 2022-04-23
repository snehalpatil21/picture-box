# picture-box
using System;
using System.Windows.Forms;
namespace manustrip107.cs
{
    public partial class Form1 : Form
    {
        int count=-1;
        public Form1()
        {
            InitializeComponent();
        }
         private void bt2_Click(object sender, EventArgs e)
        {

            if (count <= 8)
            {
                count = count + 1;
            }
            pictureBox1.SizeMode = PictureBoxSizeMode.StretchImage;
            
            pictureBox1.Image=imageList1.Images[count];
        }

        private void bt1_Click(object sender, EventArgs e)
        {
            if (count >= 0)
            {
                count = count - 1;
            }
            pictureBox1.Image = imageList1.Images[count];         }     }   } 
