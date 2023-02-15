# designing-simple-calculator-using-VB
'
' Created by SharpDevelop.
' User: BRIAN WEREH
' Date: 2/1/2023
' Time: 10:35 AM
' 
' To change this template use Tools | Options | Coding | Edit Standard Headers.
'
Public Partial Class MainForm
	Public Sub New()
		' The Me.InitializeComponent call is required for Windows Forms designer support.
		Me.InitializeComponent()
		
		'
		' TODO : Add constructor code after InitializeComponents
		'
	End Sub
	
	Sub Button3Click(sender As Object, e As EventArgs)
		Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim Sum As Single =textbox1 + textbox2
		LblAns.Text = Sum.ToString
	End Sub
	
	Sub Button4Click(sender As Object, e As EventArgs)
		Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim subtract As Single =textbox1 - textbox2
		LblAns.Text = subtract.ToString	
	End Sub
	
	Sub Button5Click(sender As Object, e As EventArgs)
		Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim multiply As Single =textbox1 * textbox2
		LblAns.Text = multiply.ToString	
	End Sub
	
	Sub Button6Click(sender As Object, e As EventArgs)
		Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim divide As Single =textbox1 / textbox2
		LblAns.Text = divide.ToString	
	End Sub
	
	Sub Button7Click(sender As Object, e As EventArgs)
		Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim Sum As Single =textbox1 \ textbox2
		LblAns.Text = Sum.ToString	
	End Sub
	
	Sub Button8Click(sender As Object, e As EventArgs)
	    Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim powerto As Single =textbox1 ^ textbox2
		LblAns.Text = powerto.ToString	
	End Sub
	
	Sub Button9Click(sender As Object, e As EventArgs)
	Dim textbox1 As Single = Val(TxtBox1.Text)
		Dim textbox2 As Single = Val(TxtBox2.Text)
		Dim remainder As Single =textbox1 Mod textbox2
		LblAns.Text = remainder.ToString	
	End Sub
	
	Sub MainFormLoad(sender As Object, e As EventArgs)
		
	End Sub
	
	Sub Button1Click(sender As Object, e As EventArgs)
		TxtBox1.clear()
		TxtBox2.clear()			
	End Sub
	
	Sub Button2Click(sender As Object, e As EventArgs)
 Dim ExitYN As System.Windows.Forms.DialogResult
 
        ExitYN = MsgBox("Do you really want to exit?", MsgBoxStyle.YesNo)
        If ExitYN = MsgBoxResult.Yes Then
            Close()
        Else
        End If
     		
	End Sub
End Class

