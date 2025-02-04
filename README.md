2, write a program to check wheather a number is odd or even.?

        Dim a As Integer
        a = TextBox1.Text
        If (a Mod 2 = 0) Then
            MsgBox("Given number is even")
        Else
            MsgBox("Given number is odd")
        End If

3, write a program to print fibonacci series.?


        Dim f0, f1, f2, n As Integer
        f0 = 0
        f1 = 1
        TextBox2.Text = f0 & "" & ""
        n = TextBox1.Text
        For i = 3 To n
            f2 = f0 + f1
            TextBox2.Text = TextBox2.Text & f2 & ""
            f0 = f1
            f1 = f2
        Next i

4, write a program to check whether a number is palindrome or not.?

        Dim a, b, r, d As Integer
        d = 0
        a = Val(TextBox1.Text)
        b = a
        While (a > 0)
            r = a Mod 10
            d = d * 10 + r
            a = a / 10
        End While

        If (d = b) Then
            Label2.Text = "Number is palindrome"
        Else
            Label2.Text = "Number is not palindrome"
        End If

5, write a program to find the sum of n numbers.?

        Dim sum, n, i As Integer
        n = TextBox1.Text
        For i = 1 To n
            sum = sum + i
        Next i
        MsgBox("The sum is " & sum)

6, Write a program to find factorial of a number.?

        Dim i, a, f As Integer
        f = 1
        i = 1
        a = TextBox1.Text
        While i <= a
            f = f * i
            i = i + 1
        End While

7, write a program for login.?

       Dim username As String, username1 As String = "bca"
       Dim password As String, password1 As String = "bca5sem"

       username = TextBox1.Text
       password = TextBox2.Text
       If username = username1 And password = password1 Then
           Label3.Text = "Success"
       Else
           Label3.Text = "Invalid username or password"
       End If

9, write a program for temperature conversion.?

        Dim a As Double
        Dim f As Double
        Dim c As Double

        a = TextBox1.Text
        If RadioButton1.Checked Then
            c = (a - 32) * 5 / 9
            Label2.Text = c & "c"
        ElseIf RadioButton2.Checked Then
            f = (a * a / 5) + 32
            Label2.Text = f & "f"
        Else
            MsgBox("Select an option")
        End If

10, write a program for calender control to display selected date.?

        Label1.Text = MonthCalendar1.SelectionStart.ToLongDateString()

11, write a program to generate quadratic equation.?

        Dim a As Double
        Dim b As Double
        Dim c, s, x1, x2 As Double

        a = TextBox1.Text
        b = TextBox2.Text
        c = TextBox3.Text
        s = Math(Sqrt(b * b - 4 * a * c))
        If (b * b - 4 * a * c) = 0 Then
            Label4.Text = "Roots are equal"
            x1 = (-b + s) / 2 * a
            x2 = (-b + s) / 2 * a
            Label4.Text = "The roots" & x1 & "or" & x2
        ElseIf (b * b - 4 * a * c) < 0 Then
            Label4.Text = "The roots are imaginary"
        Else
            Label4.Text = "The roots are not equal"
            x1 = (-b + s) / 2 * a
            x2 = (-b - s) / 2 * a
            Label4.Text = "The roots" & x1 & "or" & x2
        End If