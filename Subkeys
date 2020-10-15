CREATE TABLE composers (
    composerName varchar(20) NOT NULL,
    nationality varchar(20),
    yearOfBirth int,
    CONSTRAINT composers_pk PRIMARY KEY (composerName)
);

CREATE TABLE compositions (
    title varchar(20) NOT NULL,
    composer varchar(20) NOT NULL,
    CONSTRAINT compositions_fk FOREIGN KEY (composer)
    REFERENCES composers(composerName),
    CONSTRAINT compositions_pk PRIMARY KEY (title, composer)
);

INSERT INTO composers
VALUES  ('Beethoven', 'German', 1770),
        ('Brahms', 'German', 1841),
        ('Shostakovich', 'Russian', 1906),
        ('Mozart, W.A.', 'German', 1756),
        ('Dvorak', 'Czech', 1841);

INSERT INTO compositions
VALUES  ('Symphony #9', 'Beethoven'),
        ('Violin Concerto', 'Beethoven'),
        ('Violin Concerto', 'Brahms'),
        ('Symphony #9', 'Shostakovich'),
        ('Clarinet Concerto', 'Mozart, W.A.'),
        ('Symphony #9', 'Dvorak');