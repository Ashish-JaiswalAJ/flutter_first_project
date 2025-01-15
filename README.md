# flutter_first_project
log in page
import 'package:flutter/material.dart';


class MyHomePage extends StatelessWidget {
  const MyHomePage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: null,
      ),
      body: Container(
        width: double.infinity,
        height: double.infinity,
        decoration: BoxDecoration(
          gradient: LinearGradient(colors: [Colors.purpleAccent,Colors.deepPurple,], begin: FractionalOffset(0.0,0.0),end: FractionalOffset(1.0,1.0),)
        ),
        child: Column(
          children: [
            Image.asset('assets/images/icon.png'),
            Container(
              margin: EdgeInsets.only(top: 18),
              width: 320,
              height: 470,
              decoration: BoxDecoration(
                  gradient: LinearGradient(colors: [Colors.purpleAccent,Colors.deepPurple,], begin: FractionalOffset(0.0,0.0),end: FractionalOffset(1.0,1.0),),
                borderRadius: BorderRadius.circular(11),
                boxShadow: [BoxShadow(blurRadius:15,color: Colors.black12,spreadRadius: 3 ),]

              ),
              child: Column(mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                children: [
                  Text('Create Your Account',style: TextStyle(fontSize: 25),),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                      color: Colors.black12,
                      borderRadius: BorderRadius.circular(11)
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(8.0),
                      child: Text('Name',style: TextStyle(fontSize: 20),),
                    ),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                        color: Colors.black12,
                        borderRadius: BorderRadius.circular(11)
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(8.0),
                      child: Text('Email',style: TextStyle(fontSize: 20),),
                    ),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                        color: Colors.black12,
                        borderRadius: BorderRadius.circular(11)
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(8.0),
                      child: Text('Password',style: TextStyle(fontSize: 20),),
                    ),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                        color: Colors.black12,
                        borderRadius: BorderRadius.circular(11)
                    ),
                    child: Padding(
                      padding: const EdgeInsets.all(8.0),
                      child: Text('Confirm Password',style: TextStyle(fontSize: 20),),
                    ),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                        color: Colors.deepPurpleAccent,
                        borderRadius: BorderRadius.circular(20)
                    ),
                    child: Center(child: Text('Sign Up',style: TextStyle(fontSize: 20,),)),
                  ),

                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(

                        borderRadius: BorderRadius.circular(11)
                    ),
                    child: Row( mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                      children: [
                        Text('Already Have an account?',style: TextStyle(fontSize: 15),),
                        Text('Log in',style: TextStyle(fontSize: 20),),
                      ],
                    ),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(

                        borderRadius: BorderRadius.circular(11)
                    ),
                    child: Center(child: Text('----------------Or Sign up with----------------',style: TextStyle(fontSize: 15),)),
                  ),
                  Container(
                    height: 40,
                    width: 260,
                    decoration: BoxDecoration(
                        color: Colors.white,
                        borderRadius: BorderRadius.circular(20)
                    ),
                    child: Row( mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                      children: [
                        Text('Sign Up With Gmail',style: TextStyle(fontSize: 15),),
                      ],
                    ),
                  ),
                ],
              ),
            ),
          ],
        ),
      ),
    );
  }
}
