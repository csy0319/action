# action
<!DOCTYPE hibernate-configuration PUBLIC
	"-//Hibernate/Hibernate Configuration DTD 3.0//EN"
	"http://www.hibernate.org/dtd/hibernate-configuration-3.0.dtd">

<hibernate-configuration>
	<session-factory>
		 <!-- Database connection settings -->
        <property name="connection.driver_class">com.mysql.jdbc.Driver</property>
        <property name="connection.url">jdbc:mysql://localhost:3306/album</property>
        <property name="connection.username">root</property>
        <property name="connection.password">12345678</property>
        <property name="show_sql">true</property>
        <!-- Drop and re-create the database schema on startup -->
        <property name="hbm2ddl.auto">update</property>
      <!--   <mapping resource="model/Student.hbm.xml"/> -->
      <mapping class="net.csy.entity.User"/>

	</session-factory>
</hibernate-configuration>
