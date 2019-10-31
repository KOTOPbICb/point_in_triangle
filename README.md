Это не ЛУА БЛЯТЬ! Это Си
```
BOOL IsInTriangle( VEC P1, VEC P2, VEC P3, VEC PTest )
{
  int a = (P1.X - PTest.X) * (P2.Y - P1.Y) - (P2.X - P1.X) * (P1.Y - PTest.Y);
  int b = (P2.X - PTest.X) * (P3.Y - P2.Y) - (P3.X - P2.X) * (P2.Y - PTest.Y);
  int c = (P3.X - PTest.X) * (P1.Y - P3.Y) - (P1.X - P3.X) * (P3.Y - PTest.Y);
 
  if ((a >= 0 && b >= 0 && c >= 0) || (a <= 0 && b <= 0 && c <= 0))
    return TRUE;
  else
    return FALSE;
}
