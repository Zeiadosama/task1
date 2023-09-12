import 'package:flutter/material.dart';

void main() {
  runApp(const ZEDApp());
}

class ZEDApp extends StatelessWidget {
  const ZEDApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        backgroundColor: Colors.purple,
        appBar: AppBar(
          backgroundColor: Colors.black,
          leading: const Icon(
            Icons.add_alert_sharp,
          ),
          centerTitle: true,
          title: const Text("ZED App"),
          actions: const [],
        ),
        body: SingleChildScrollView(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.start,
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
              Text("zeiad"),
              Icon(Icons.add_alert_sharp),
              Row(children: [
                Icon(
                  Icons.access_time,
                ),
                Icon(Icons.add_alert_sharp),
                Icon(Icons.access_time),
                Icon(Icons.add_a_photo),
              ]),
              Image.network(
                  "https://static.vecteezy.com/system/resources/previews/009/273/280/non_2x/concept-of-loneliness-and-disappointment-in-love-sad-man-sitting-element-of-the-picture-is-decorated-by-nasa-free-photo.jpg"),
              Text("icthub"),
              const SizedBox(
                height: 700, ),


                 SizedBox(
                   height: 200,
                     child:Image.asset("Img1.jpg")
                ),
                 

            ],
          ),
        ),
      ),
    );
  }
}
