
public static void write() throws IOException
  {
  OutputStreamWriter osw1 = new OutputStreamWriter(new FileOutputStream("gbk.txt"),"G
  osw1.close();
  
  OutputStreamWriter osw2 = new OutputStreamWriter(new FileOutputStream("utf-8.txt"),"UTF-8");
  osw2.write("ÄãºÃ");
  osw2.close();
 }
 public static void rea
 {
 InputStreamReader isr = new InputStreamReader(new FileInputStream("gbk.txt"),"GBK");
 byte[] buf = new byte[1024];
 int len = isr.read(buf);
 sop(new String(buf,0,len));
 }
ghjhgjhjhj
