# jsp_JNDI
java Naming Directory interface

public class BaseDao{
	public Connection con=null;
	public Connection getcon(){
		Context intico=new InitialContext();
		DataSource ds=(DataSource)intico.lookup("java:comp/env/jdbc/news");
			con=ds.getConnection();
	}
  
}
