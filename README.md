# decimalToBinary



string DecimalToBinary(ll num)
{
    string str;
    if(num==0)
        return 0;
    while(num)
    {
        if(num & 1)
            str+='1';
        else
            str+='0';
          num>>=1;
    }   
    string s = str;
    reverse(all(s));
    return s;
}
