Public Class frmCalc

    Private Sub btnPlus_Click(sender As Object, e As EventArgs) Handles btnPlus.Click
        txtAnswer.Text = Val(txtFirst.Text) + Val(txtSecond.Text)
    End Sub

    Private Sub btnMinus_Click(sender As Object, e As EventArgs) Handles btnMinus.Click
        txtAnswer.Text = txtFirst.Text - txtSecond.Text
    End Sub

    Private Sub btnMultiply_Click(sender As Object, e As EventArgs) Handles btnMultiply.Click
        txtAnswer.Text = txtFirst.Text * txtSecond.Text
    End Sub

    Private Sub btnDivide_Click(sender As Object, e As EventArgs) Handles btnDivide.Click
        txtAnswer.Text = txtFirst.Text / txtSecond.Text
    End Sub

    Private Sub btnMod_Click(sender As Object, e As EventArgs) Handles btnMod.Click
        txtAnswer.Text = txtFirst.Text Mod txtSecond.Text
    End Sub

    Private Sub btnClear_Click(sender As Object, e As EventArgs) Handles btnClear.Click
        txtFirst.Text = ""
        txtSecond.Text = ""
        txtAnswer.Text = ""
        txtFirst.Focus()
    End Sub

    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        Me.Close()
    End Sub
End Class
