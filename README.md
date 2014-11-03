Blog menggunakan PHP dan MySQL
=========


Contoh sederhana dari pembuatan blog menggunakan PHP dan MySQL. Anda harus membuat database dengan nama "blog" kemudian membuat sebuah membuat sebuah tabel post untuk menampung data tulisan.

```sh
CREATE TABLE `posts` (
  `post_id` int(4) NOT NULL AUTO_INCREMENT,
  `title` varchar(250) NOT NULL,
  `date` date NOT NULL,
  `content` text NOT NULL,
  `deleted` int(1) NOT NULL DEFAULT '0',
  PRIMARY KEY (`post_id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;

```

Kemudhan membuat sebuah dummy data seperti dibawah ini.

```sh
INSERT INTO `posts` VALUES(1, 'Postingan Pertama', '2014-10-28', 'ini adalah tulisan pertama untuk demo blogpost\n\nFar far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia.\n\nIt is a paradisematic country, in which roasted parts of sentences fly into your mouth. Even the all-powerful Pointing has no control about the blind texts it is an almost unorthographic life One day however a small line of blind text by the name of Lorem Ipsum decided to leave for the far World of Grammar. ', 0);
INSERT INTO `posts` VALUES(2, 'Tulisan Kedua', '2014-10-29', 'ini adalah tulisan kedua untuk demo blogpost\n\nFar far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia.\n\nIt is a paradisematic country, in which roasted parts of sentences fly into your mouth. Even the all-powerful Pointing has no control about the blind texts it is an almost unorthographic life One day however a small line of blind text by the name of Lorem Ipsum decided to leave for the far World of Grammar. ', 0);

```

License
=========
MIT
