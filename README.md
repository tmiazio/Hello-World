Public Class Calc

    Dim val1 As String = ""
    Dim val2 As String = ""
    Dim val3 As String = "0.0"
    Private Sub ClearDisplay()
        displayBox.Clear()
    End Sub

    Private Sub clearDis_Click(sender As Object, e As EventArgs) Handles clearDis.Click
        ClearDisplay()
    End Sub

    Private Sub clearButton_Click(sender As Object, e As EventArgs) Handles clearButton.Click
        ClearDisplay()
    End Sub

    Private Sub exitCalc_Click(sender As Object, e As EventArgs) Handles exitCalc.Click
        End
    End Sub

    Private Sub number0_Click(sender As Object, e As EventArgs) Handles number0.Click
        If displayBox.Text = val1 Then
            displayBox.Text = "0"
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = "0"
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = "0"
        ElseIf displayBox.Text = val1 Then
            displayBox.Text = "0"
        Else : displayBox.Text = displayBox.Text & "0"
        End If
    End Sub

    Private Sub number1_Click(sender As Object, e As EventArgs) Handles number1.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number2_Click(sender As Object, e As EventArgs) Handles number2.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number3_Click(sender As Object, e As EventArgs) Handles number3.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number4_Click(sender As Object, e As EventArgs) Handles number4.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number5_Click(sender As Object, e As EventArgs) Handles number5.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number6_Click(sender As Object, e As EventArgs) Handles number6.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number7_Click(sender As Object, e As EventArgs) Handles number7.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number8_Click(sender As Object, e As EventArgs) Handles number8.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub number9_Click(sender As Object, e As EventArgs) Handles number9.Click
        If displayBox.Text = val1 Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = "0" Then
            displayBox.Text = sender.Text
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = sender.Text
        Else
            displayBox.Text = displayBox.Text & sender.Text
        End If
    End Sub

    Private Sub decimalButton_Click(sender As Object, e As EventArgs) Handles decimalButton.Click
        If displayBox.Text = "0" Then
            displayBox.Text = "."
        ElseIf displayBox.Text = val3 Then
            displayBox.Text = "."
        ElseIf displayBox.Text = val1 Then
            displayBox.Text = "."
        Else
            If displayBox.Text.Contains(".") Then
            Else
                displayBox.Text = displayBox.Text & "."
            End If
        End If
    End Sub

    Private Sub addButton_Click(sender As Object, e As EventArgs) Handles addButton.Click
        val2 = sender.Text
        val1 = displayBox.Text
    End Sub

    Private Sub subtractButton_Click(sender As Object, e As EventArgs) Handles subtractButton.Click
        val2 = sender.Text
        val1 = displayBox.Text
    End Sub

    Private Sub multiplyButton_Click(sender As Object, e As EventArgs) Handles multiplyButton.Click
        val2 = sender.Text
        val1 = displayBox.Text
    End Sub

    Private Sub divideButton_Click(sender As Object, e As EventArgs) Handles divideButton.Click
        val2 = sender.Text
        val1 = displayBox.Text
    End Sub

    Private Sub equalsButton_Click(sender As Object, e As EventArgs) Handles equalsButton.Click
        If val1 > "" And val2 = "+" Then
            displayBox.Text = Val(val1) + Val(displayBox.Text)
            val3 = displayBox.Text
        ElseIf val2 > "" And val2 = "-" Then
            displayBox.Text = Val(val1) - Val(displayBox.Text)
            val3 = displayBox.Text
        ElseIf val2 > "" And val2 = "x" Then
            displayBox.Text = Val(val1) * Val(displayBox.Text)
            val3 = displayBox.Text
        ElseIf val2 > "" And val2 = "/" Then
            displayBox.Text = Val(val1) / Val(displayBox.Text)
            val3 = displayBox.Text
        End If
    End Sub
End Class
