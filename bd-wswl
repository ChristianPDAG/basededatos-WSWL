-- phpMyAdmin SQL Dump
-- version 5.2.0
-- https://www.phpmyadmin.net/
--
-- Servidor: 127.0.0.1
-- Tiempo de generación: 14-10-2022 a las 17:52:20
-- Versión del servidor: 10.4.25-MariaDB
-- Versión de PHP: 8.1.10

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de datos: `pruebadb`
--

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `admin`
--

CREATE TABLE `admin` (
  `ID_ADMIN` int(11) NOT NULL,
  `NAME_ADMIN` varchar(50) NOT NULL,
  `PHONE` int(11) NOT NULL,
  `MAIL` varchar(40) NOT NULL,
  `ID_CITY` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `admin`
--

INSERT INTO `admin` (`ID_ADMIN`, `NAME_ADMIN`, `PHONE`, `MAIL`, `ID_CITY`) VALUES
(1, 'delphine', 995, 'dchristou0@nyu.edu', 25),
(2, 'dane', 206, 'dfontanet1@github.io', 18),
(3, 'meryl', 277, 'mbridgwood2@google.ru', 1),
(4, 'ashlen', 249, 'awoloschinski3@sfgate.com', 1),
(5, 'jackson', 895, 'jcliss4@apache.org', 12),
(6, 'barron', 801, 'bhuggons5@state.tx.us', 8),
(7, 'mariam', 373, 'mfrye6@salon.com', 7),
(8, 'estrellita', 390, 'ebolle7@google.it', 16),
(9, 'bryce', 162, 'bsmieton8@blogs.com', 8),
(10, 'merry', 780, 'mtearny9@geocities.com', 17);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `alert`
--

CREATE TABLE `alert` (
  `ID_ALERT` int(11) NOT NULL,
  `NAME` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `alert`
--

INSERT INTO `alert` (`ID_ALERT`, `NAME`) VALUES
(1, 'Verde'),
(2, 'Amarillo'),
(3, 'Naranjo'),
(4, 'Rojo');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `ambient_data`
--

CREATE TABLE `ambient_data` (
  `ID_AD` int(11) NOT NULL,
  `TEMPERATURE` float NOT NULL,
  `HUMIDITY` float NOT NULL,
  `DECIBEL` float NOT NULL,
  `PPM` float NOT NULL,
  `DATE` date NOT NULL,
  `ID_STATUS` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `ambient_data`
--

INSERT INTO `ambient_data` (`ID_AD`, `TEMPERATURE`, `HUMIDITY`, `DECIBEL`, `PPM`, `DATE`, `ID_STATUS`) VALUES
(1, 8.01, 0, 494.83, 519.92, '0000-00-00', 3),
(2, 2.14, 0, 321.57, 359.93, '2022-04-10', 1),
(4, 41.14, 0, 272.56, 426.49, '0000-00-00', 2),
(5, 37.45, 0, 684.25, 344.25, '0000-00-00', 4),
(6, 35.91, 0, 965.74, 950.53, '2022-02-23', 3),
(7, 8.24, 0, 445.08, 152.87, '0000-00-00', 1),
(8, 31.31, 0, 851.49, 316.99, '2022-09-17', 1),
(10, 31.26, 0, 600.82, 827.87, '2022-08-10', 3);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `caregiver`
--

CREATE TABLE `caregiver` (
  `ID_CAREGIVER` int(11) NOT NULL,
  `NAME` varchar(40) NOT NULL,
  `PHONE` int(11) NOT NULL,
  `MAIL` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `caregiver`
--

INSERT INTO `caregiver` (`ID_CAREGIVER`, `NAME`, `PHONE`, `MAIL`) VALUES
(1, 'amabelle', 420, 'avillalta0@symantec.com'),
(2, 'bryanty', 86, 'bmatches1@sogou.com'),
(3, 'elfrida', 63, 'espracklin2@boston.com'),
(4, 'robinet', 48, 'rbancroft3@cbc.ca'),
(5, 'kaitlin', 86, 'krumford4@soup.io'),
(6, 'lindi', 351, 'lnicholls5@slate.com'),
(7, 'norton', 62, 'ncrocetto6@de.vu'),
(8, 'susi', 86, 'sdudgeon7@wired.com'),
(9, 'moore', 380, 'mseifenmacher8@nydailynews.com'),
(10, 'charley', 51, 'cmounsey9@goo.gl');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `city`
--

CREATE TABLE `city` (
  `ID_CITY` int(11) NOT NULL,
  `CITY` varchar(40) NOT NULL,
  `ID_PROVINCE` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `city`
--

INSERT INTO `city` (`ID_CITY`, `CITY`, `ID_PROVINCE`) VALUES
(1, 'Arica', 1),
(2, 'Camarones', 1),
(3, 'General Lagos', 2),
(4, 'Putre', 2),
(5, 'Alto Hospicio', 3),
(6, 'Iquique', 3),
(7, 'Camiña', 4),
(8, 'Colchane', 4),
(9, 'Huara', 4),
(10, 'Pica', 4),
(11, 'Pozo Almonte', 4),
(12, 'Antofagasta', 5),
(13, 'Mejillones', 5),
(14, 'Sierra Gorda', 5),
(15, 'Taltal', 5),
(16, 'Calama', 6),
(17, 'Ollague', 6),
(18, 'San Pedro de Atacama', 6),
(19, 'María Elena', 7),
(20, 'Tocopilla', 7),
(21, 'Chañaral', 8),
(22, 'Diego de Almagro', 8),
(23, 'Caldera', 9),
(24, 'Copiapó', 9),
(25, 'Tierra Amarilla', 9),
(26, 'Alto del Carmen', 10),
(27, 'Freirina', 10),
(28, 'Huasco', 10),
(29, 'Vallenar', 10),
(30, 'Canela', 11),
(31, 'Illapel', 11),
(32, 'Los Vilos', 11),
(33, 'Salamanca', 11),
(34, 'Andacollo', 12),
(35, 'Coquimbo', 12),
(36, 'La Higuera', 12),
(37, 'La Serena', 12),
(38, 'Paihuaco', 12),
(39, 'Vicuña', 12),
(40, 'Combarbalá', 13),
(41, 'Monte Patria', 13),
(42, 'Ovalle', 13),
(43, 'Punitaqui', 13),
(44, 'Río Hurtado', 13),
(45, 'Isla de Pascua', 14),
(46, 'Calle Larga', 15),
(47, 'Los Andes', 15),
(48, 'Rinconada', 15),
(49, 'San Esteban', 15),
(50, 'La Ligua', 16),
(51, 'Papudo', 16),
(52, 'Petorca', 16),
(53, 'Zapallar', 16),
(54, 'Hijuelas', 17),
(55, 'La Calera', 17),
(56, 'La Cruz', 17),
(57, 'Limache', 17),
(58, 'Nogales', 17),
(59, 'Olmué', 17),
(60, 'Quillota', 17),
(61, 'Algarrobo', 18),
(62, 'Cartagena', 18),
(63, 'El Quisco', 18),
(64, 'El Tabo', 18),
(65, 'San Antonio', 18),
(66, 'Santo Domingo', 18),
(67, 'Catemu', 19),
(68, 'Llaillay', 19),
(69, 'Panquehue', 19),
(70, 'Putaendo', 19),
(71, 'San Felipe', 19),
(72, 'Santa María', 19),
(73, 'Casablanca', 20),
(74, 'Concón', 20),
(75, 'Juan Fernández', 20),
(76, 'Puchuncaví', 20),
(77, 'Quilpué', 20),
(78, 'Quintero', 20),
(79, 'Valparaíso', 20),
(80, 'Villa Alemana', 20),
(81, 'Viña del Mar', 20),
(82, 'Colina', 21),
(83, 'Lampa', 21),
(84, 'Tiltil', 21),
(85, 'Pirque', 22),
(86, 'Puente Alto', 22),
(87, 'San José de Maipo', 22),
(88, 'Buin', 23),
(89, 'Calera de Tango', 23),
(90, 'Paine', 23),
(91, 'San Bernardo', 23),
(92, 'Alhué', 24),
(93, 'Curacaví', 24),
(94, 'María Pinto', 24),
(95, 'Melipilla', 24),
(96, 'San Pedro', 24),
(97, 'Cerrillos', 25),
(98, 'Cerro Navia', 25),
(99, 'Conchalí', 25),
(100, 'El Bosque', 25),
(101, 'Estación Central', 25),
(102, 'Huechuraba', 25),
(103, 'Independencia', 25),
(104, 'La Cisterna', 25),
(105, 'La Granja', 25),
(106, 'La Florida', 25),
(107, 'La Pintana', 25),
(108, 'La Reina', 25),
(109, 'Las Condes', 25),
(110, 'Lo Barnechea', 25),
(111, 'Lo Espejo', 25),
(112, 'Lo Prado', 25),
(113, 'Macul', 25),
(114, 'Maipú', 25),
(115, 'Ñuñoa', 25),
(116, 'Pedro Aguirre Cerda', 25),
(117, 'Peñalolén', 25),
(118, 'Providencia', 25),
(119, 'Pudahuel', 25),
(120, 'Quilicura', 25),
(121, 'Quinta Normal', 25),
(122, 'Recoleta', 25),
(123, 'Renca', 25),
(124, 'San Miguel', 25),
(125, 'San Joaquín', 25),
(126, 'San Ramón', 25),
(127, 'Santiago', 25),
(128, 'Vitacura', 25),
(129, 'El Monte', 26),
(130, 'Isla de Maipo', 26),
(131, 'Padre Hurtado', 26),
(132, 'Peñaflor', 26),
(133, 'Talagante', 26),
(134, 'Codegua', 27),
(135, 'Coínco', 27),
(136, 'Coltauco', 27),
(137, 'Doñihue', 27),
(138, 'Graneros', 27),
(139, 'Las Cabras', 27),
(140, 'Machalí', 27),
(141, 'Malloa', 27),
(142, 'Mostazal', 27),
(143, 'Olivar', 27),
(144, 'Peumo', 27),
(145, 'Pichidegua', 27),
(146, 'Quinta de Tilcoco', 27),
(147, 'Rancagua', 27),
(148, 'Rengo', 27),
(149, 'Requínoa', 27),
(150, 'San Vicente de Tagua Tagua', 27),
(151, 'La Estrella', 28),
(152, 'Litueche', 28),
(153, 'Marchihue', 28),
(154, 'Navidad', 28),
(155, 'Peredones', 28),
(156, 'Pichilemu', 28),
(157, 'Chépica', 29),
(158, 'Chimbarongo', 29),
(159, 'Lolol', 29),
(160, 'Nancagua', 29),
(161, 'Palmilla', 29),
(162, 'Peralillo', 29),
(163, 'Placilla', 29),
(164, 'Pumanque', 29),
(165, 'San Fernando', 29),
(166, 'Santa Cruz', 29),
(167, 'Cauquenes', 30),
(168, 'Chanco', 30),
(169, 'Pelluhue', 30),
(170, 'Curicó', 31),
(171, 'Hualañé', 31),
(172, 'Licantén', 31),
(173, 'Molina', 31),
(174, 'Rauco', 31),
(175, 'Romeral', 31),
(176, 'Sagrada Familia', 31),
(177, 'Teno', 31),
(178, 'Vichuquén', 31),
(179, 'Colbún', 32),
(180, 'Linares', 32),
(181, 'Longaví', 32),
(182, 'Parral', 32),
(183, 'Retiro', 32),
(184, 'San Javier', 32),
(185, 'Villa Alegre', 32),
(186, 'Yerbas Buenas', 32),
(187, 'Constitución', 33),
(188, 'Curepto', 33),
(189, 'Empedrado', 33),
(190, 'Maule', 33),
(191, 'Pelarco', 33),
(192, 'Pencahue', 33),
(193, 'Río Claro', 33),
(194, 'San Clemente', 33),
(195, 'San Rafael', 33),
(196, 'Talca', 33),
(197, 'Arauco', 34),
(198, 'Cañete', 34),
(199, 'Contulmo', 34),
(200, 'Curanilahue', 34),
(201, 'Lebu', 34),
(202, 'Los Álamos', 34),
(203, 'Tirúa', 34),
(204, 'Alto Biobío', 35),
(205, 'Antuco', 35),
(206, 'Cabrero', 35),
(207, 'Laja', 35),
(208, 'Los Ángeles', 35),
(209, 'Mulchén', 35),
(210, 'Nacimiento', 35),
(211, 'Negrete', 35),
(212, 'Quilaco', 35),
(213, 'Quilleco', 35),
(214, 'San Rosendo', 35),
(215, 'Santa Bárbara', 35),
(216, 'Tucapel', 35),
(217, 'Yumbel', 35),
(218, 'Chiguayante', 36),
(219, 'Concepción', 36),
(220, 'Coronel', 36),
(221, 'Florida', 36),
(222, 'Hualpén', 36),
(223, 'Hualqui', 36),
(224, 'Lota', 36),
(225, 'Penco', 36),
(226, 'San Pedro de La Paz', 36),
(227, 'Santa Juana', 36),
(228, 'Talcahuano', 36),
(229, 'Tomé', 36),
(230, 'Bulnes', 37),
(231, 'Chillán', 37),
(232, 'Chillán Viejo', 37),
(233, 'Cobquecura', 37),
(234, 'Coelemu', 37),
(235, 'Coihueco', 37),
(236, 'El Carmen', 37),
(237, 'Ninhue', 37),
(238, 'Ñiquen', 37),
(239, 'Pemuco', 37),
(240, 'Pinto', 37),
(241, 'Portezuelo', 37),
(242, 'Quillón', 37),
(243, 'Quirihue', 37),
(244, 'Ránquil', 37),
(245, 'San Carlos', 37),
(246, 'San Fabián', 37),
(247, 'San Ignacio', 37),
(248, 'San Nicolás', 37),
(249, 'Treguaco', 37),
(250, 'Yungay', 37),
(251, 'Carahue', 38),
(252, 'Cholchol', 38),
(253, 'Cunco', 38),
(254, 'Curarrehue', 38),
(255, 'Freire', 38),
(256, 'Galvarino', 38),
(257, 'Gorbea', 38),
(258, 'Lautaro', 38),
(259, 'Loncoche', 38),
(260, 'Melipeuco', 38),
(261, 'Nueva Imperial', 38),
(262, 'Padre Las Casas', 38),
(263, 'Perquenco', 38),
(264, 'Pitrufquén', 38),
(265, 'Pucón', 38),
(266, 'Saavedra', 38),
(267, 'Temuco', 38),
(268, 'Teodoro Schmidt', 38),
(269, 'Toltén', 38),
(270, 'Vilcún', 38),
(271, 'Villarrica', 38),
(272, 'Angol', 39),
(273, 'Collipulli', 39),
(274, 'Curacautín', 39),
(275, 'Ercilla', 39),
(276, 'Lonquimay', 39),
(277, 'Los Sauces', 39),
(278, 'Lumaco', 39),
(279, 'Purén', 39),
(280, 'Renaico', 39),
(281, 'Traiguén', 39),
(282, 'Victoria', 39),
(283, 'Corral', 40),
(284, 'Lanco', 40),
(285, 'Los Lagos', 40),
(286, 'Máfil', 40),
(287, 'Mariquina', 40),
(288, 'Paillaco', 40),
(289, 'Panguipulli', 40),
(290, 'Valdivia', 40),
(291, 'Futrono', 41),
(292, 'La Unión', 41),
(293, 'Lago Ranco', 41),
(294, 'Río Bueno', 41),
(295, 'Ancud', 42),
(296, 'Castro', 42),
(297, 'Chonchi', 42),
(298, 'Curaco de Vélez', 42),
(299, 'Dalcahue', 42),
(300, 'Puqueldón', 42),
(301, 'Queilén', 42),
(302, 'Quemchi', 42),
(303, 'Quellón', 42),
(304, 'Quinchao', 42),
(305, 'Calbuco', 43),
(306, 'Cochamó', 43),
(307, 'Fresia', 43),
(308, 'Frutillar', 43),
(309, 'Llanquihue', 43),
(310, 'Los Muermos', 43),
(311, 'Maullín', 43),
(312, 'Puerto Montt', 43),
(313, 'Puerto Varas', 43),
(314, 'Osorno', 44),
(315, 'Puero Octay', 44),
(316, 'Purranque', 44),
(317, 'Puyehue', 44),
(318, 'Río Negro', 44),
(319, 'San Juan de la Costa', 44),
(320, 'San Pablo', 44),
(321, 'Chaitén', 45),
(322, 'Futaleufú', 45),
(323, 'Hualaihué', 45),
(324, 'Palena', 45),
(325, 'Aisén', 46),
(326, 'Cisnes', 46),
(327, 'Guaitecas', 46),
(328, 'Cochrane', 47),
(329, 'O\'higgins', 47),
(330, 'Tortel', 47),
(331, 'Coihaique', 48),
(332, 'Lago Verde', 48),
(333, 'Chile Chico', 49),
(334, 'Río Ibáñez', 49),
(335, 'Antártica', 50),
(336, 'Cabo de Hornos', 50),
(337, 'Laguna Blanca', 51),
(338, 'Punta Arenas', 51),
(339, 'Río Verde', 51),
(340, 'San Gregorio', 51),
(341, 'Porvenir', 52),
(342, 'Primavera', 52),
(343, 'Timaukel', 52),
(344, 'Natales', 53),
(345, 'Torres del Paine', 53);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `condition_p`
--

CREATE TABLE `condition_p` (
  `ID_CONDITION` int(11) NOT NULL,
  `NAME_CONDITION` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `condition_p`
--

INSERT INTO `condition_p` (`ID_CONDITION`, `NAME_CONDITION`) VALUES
(0, 'depression in the elderly'),
(1, 'depression in the elderly'),
(2, 'Alzheimer´s'),
(3, 'Ictus'),
(4, 'Heart attack'),
(5, 'osteoarthritis and arthritis'),
(6, 'Hypertension'),
(7, 'Parkinson´s'),
(8, 'waterfalls'),
(9, 'osteoporosis'),
(10, 'fibromyalgia');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `device`
--

CREATE TABLE `device` (
  `ID_DEVICE` varchar(40) NOT NULL,
  `ID_LOCATION` int(11) NOT NULL,
  `ID_AD` int(11) NOT NULL,
  `SECTOR` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `device`
--

INSERT INTO `device` (`ID_DEVICE`, `ID_LOCATION`, `ID_AD`, `SECTOR`) VALUES
('70:ee:50:96:9b:1e', 5, 2, 'ambiente 1');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `emergency_contact`
--

CREATE TABLE `emergency_contact` (
  `ID_EC` int(11) NOT NULL,
  `NAME` varchar(40) NOT NULL,
  `PHONE` int(11) NOT NULL,
  `MAIL` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `emergency_contact`
--

INSERT INTO `emergency_contact` (`ID_EC`, `NAME`, `PHONE`, `MAIL`) VALUES
(1, 'Juan Alberto Rodriguez Orellana', 99563598, 'Juan.Alberto@gmail.com'),
(2, 'Cristina Andrea Perez Segovia', 78586235, 'cristinaperez@hotmail.com'),
(3, 'Roberto Manuel Riquelme Riquelme', 98663365, 'robertoriquelme@gmail.com'),
(4, 'Andrea Paz Riquelme Segovia', 75866635, 'andrea.riquelme@hotmail.com');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `location`
--

CREATE TABLE `location` (
  `ID_LOCATION` int(11) NOT NULL,
  `ID_CITY` int(11) NOT NULL,
  `ADDRESS` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `location`
--

INSERT INTO `location` (`ID_LOCATION`, `ID_CITY`, `ADDRESS`) VALUES
(1, 1, '945 american ash trail'),
(2, 9, '98 basil drive'),
(3, 8, '889 comanche trail'),
(4, 9, '019 iowa trail'),
(5, 4, '9835 merchant hill'),
(6, 5, '0945 columbus point'),
(7, 1, '582 crownhardt road'),
(8, 1, '1 debra plaza'),
(9, 9, '972 dorton hill'),
(10, 3, '01 darwin circle');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `patient`
--

CREATE TABLE `patient` (
  `ID_PATIENT` int(11) NOT NULL,
  `NAME` varchar(40) NOT NULL,
  `BIRTH_DATE` date NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `patient`
--

INSERT INTO `patient` (`ID_PATIENT`, `NAME`, `BIRTH_DATE`) VALUES
(1, 'kelly sivier', '0000-00-00'),
(2, 'hillard perle', '0000-00-00'),
(3, 'mathew meriguet', '0000-00-00'),
(4, 'querida tallon', '0000-00-00'),
(5, 'xerxes brundrett', '0000-00-00'),
(6, 'timothy ambrogio', '0000-00-00'),
(7, 'marcille freeman', '1952-09-22'),
(8, 'johnnie baline', '1952-09-22'),
(9, 'hartley tamblyn', '1952-09-22'),
(10, 'reinwald fairfoul', '1952-09-23');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `patient_condition`
--

CREATE TABLE `patient_condition` (
  `ID_PC` int(11) NOT NULL,
  `ID_PATIENT` int(11) NOT NULL,
  `ID_CONDITION` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `patient_condition`
--

INSERT INTO `patient_condition` (`ID_PC`, `ID_PATIENT`, `ID_CONDITION`) VALUES
(1, 2, 7),
(2, 8, 3);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `patient_service`
--

CREATE TABLE `patient_service` (
  `ID_PS` int(11) NOT NULL,
  `ID_DEVICE` varchar(40) NOT NULL,
  `ID_PATIENT` int(11) NOT NULL,
  `ID_CAREGIVER` int(11) NOT NULL,
  `ID_ADMIN` int(11) NOT NULL,
  `ID_SPA` int(11) NOT NULL,
  `ID_EC` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `patient_service`
--

INSERT INTO `patient_service` (`ID_PS`, `ID_DEVICE`, `ID_PATIENT`, `ID_CAREGIVER`, `ID_ADMIN`, `ID_SPA`, `ID_EC`) VALUES
(1, '70:ee:50:96:9b:1e', 2, 1, 7, 4, 1),
(2, '70:ee:50:96:9b:1e', 8, 5, 3, 3, 4);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `province`
--

CREATE TABLE `province` (
  `ID_PROVINCE` int(11) NOT NULL,
  `PROVINCE` varchar(40) NOT NULL,
  `ID_REGION` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `province`
--

INSERT INTO `province` (`ID_PROVINCE`, `PROVINCE`, `ID_REGION`) VALUES
(1, 'Arica', 1),
(2, 'Parinacota', 1),
(3, 'Iquique', 2),
(4, 'El Tamarugal', 2),
(5, 'Antofagasta', 3),
(6, 'El Loa', 3),
(7, 'Tocopilla', 3),
(8, 'Chañaral', 4),
(9, 'Copiapó', 4),
(10, 'Huasco', 4),
(11, 'Choapa', 5),
(12, 'Elqui', 5),
(13, 'Limarí', 5),
(14, 'Isla de Pascua', 6),
(15, 'Los Andes', 6),
(16, 'Petorca', 6),
(17, 'Quillota', 6),
(18, 'San Antonio', 6),
(19, 'San Felipe de Aconcagua', 6),
(20, 'Valparaiso', 6),
(21, 'Chacabuco', 7),
(22, 'Cordillera', 7),
(23, 'Maipo', 7),
(24, 'Melipilla', 7),
(25, 'Santiago', 7),
(26, 'Talagante', 7),
(27, 'Cachapoal', 8),
(28, 'Cardenal Caro', 8),
(29, 'Colchagua', 8),
(30, 'Cauquenes', 9),
(31, 'Curicó', 9),
(32, 'Linares', 9),
(33, 'Talca', 9),
(34, 'Arauco', 10),
(35, 'Bio Bío', 10),
(36, 'Concepción', 10),
(37, 'Ñuble', 10),
(38, 'Cautín', 11),
(39, 'Malleco', 11),
(40, 'Valdivia', 12),
(41, 'Ranco', 12),
(42, 'Chiloé', 13),
(43, 'Llanquihue', 13),
(44, 'Osorno', 13),
(45, 'Palena', 13),
(46, 'Aisén', 14),
(47, 'Capitán Prat', 14),
(48, 'Coihaique', 14),
(49, 'General Carrera', 14),
(50, 'Antártica Chilena', 15),
(51, 'Magallanes', 15),
(52, 'Tierra del Fuego', 15),
(53, 'Última Esperanza', 15);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `region`
--

CREATE TABLE `region` (
  `ID_REGION` int(11) NOT NULL,
  `REGION` varchar(40) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `region`
--

INSERT INTO `region` (`ID_REGION`, `REGION`) VALUES
(1, 'Arica y Parinacota'),
(2, 'Tarapacá'),
(3, 'Antofagasta'),
(4, 'Atacama'),
(5, 'Coquimbo'),
(6, 'Valparaiso'),
(7, 'Metropolitana de Santiago'),
(8, 'Libertador General Bernardo OHiggins'),
(9, 'Maule'),
(10, 'Biobío'),
(11, 'La Araucanía'),
(12, 'Los Ríos'),
(13, 'Los Lagos'),
(14, 'Aisén del General Carlos Ibáñez del Camp'),
(15, 'Magallanes y de la Antártica Chilena');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `resolution`
--

CREATE TABLE `resolution` (
  `ID_RA` int(11) NOT NULL,
  `COMMENT_R` varchar(50) NOT NULL,
  `DATE_R` date NOT NULL,
  `ID_SPA` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `resolution`
--

INSERT INTO `resolution` (`ID_RA`, `COMMENT_R`, `DATE_R`, `ID_SPA`) VALUES
(1, 'middleware', '0000-00-00', 6),
(2, 'ameliorated optimizing attitude', '0000-00-00', 4),
(3, 'monitored fault-tolerant architecture', '0000-00-00', 8),
(4, 'customizable tertiary collaboration', '0000-00-00', 5),
(5, 'secured stable structure', '0000-00-00', 8),
(6, 'fully-configurable bi-directional utilisation', '0000-00-00', 2),
(7, 'user-friendly web-enabled function', '0000-00-00', 4),
(8, 'reverse-engineered dynamic structure', '0000-00-00', 1),
(9, 'ergonomic non-volatile core', '0000-00-00', 7),
(10, 'streamlined local customer loyalty', '0000-00-00', 1);

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `sp_alert`
--

CREATE TABLE `sp_alert` (
  `ID_SPA` int(11) NOT NULL,
  `ID_ALERT` int(11) NOT NULL,
  `DATE` date NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `sp_alert`
--

INSERT INTO `sp_alert` (`ID_SPA`, `ID_ALERT`, `DATE`) VALUES
(0, 2, '0000-00-00'),
(1, 1, '0000-00-00'),
(2, 2, '0000-00-00'),
(3, 3, '0000-00-00'),
(4, 4, '0000-00-00'),
(5, 1, '0000-00-00'),
(6, 2, '0000-00-00'),
(7, 3, '0000-00-00'),
(8, 4, '0000-00-00');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `status`
--

CREATE TABLE `status` (
  `ID_STATUS` int(11) NOT NULL,
  `NAME_STATUS` varchar(50) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Volcado de datos para la tabla `status`
--

INSERT INTO `status` (`ID_STATUS`, `NAME_STATUS`) VALUES
(1, ' emergency '),
(2, ' bad '),
(3, ' good '),
(4, ' Excellent');

--
-- Índices para tablas volcadas
--

--
-- Indices de la tabla `admin`
--
ALTER TABLE `admin`
  ADD PRIMARY KEY (`ID_ADMIN`),
  ADD KEY `ID_ADMIN_FK0` (`ID_CITY`);

--
-- Indices de la tabla `alert`
--
ALTER TABLE `alert`
  ADD PRIMARY KEY (`ID_ALERT`);

--
-- Indices de la tabla `ambient_data`
--
ALTER TABLE `ambient_data`
  ADD PRIMARY KEY (`ID_AD`),
  ADD KEY `AMBIENT_DATA_FK0` (`ID_STATUS`);

--
-- Indices de la tabla `caregiver`
--
ALTER TABLE `caregiver`
  ADD PRIMARY KEY (`ID_CAREGIVER`);

--
-- Indices de la tabla `city`
--
ALTER TABLE `city`
  ADD PRIMARY KEY (`ID_CITY`),
  ADD KEY `CITY_FK0` (`ID_PROVINCE`);

--
-- Indices de la tabla `condition_p`
--
ALTER TABLE `condition_p`
  ADD PRIMARY KEY (`ID_CONDITION`);

--
-- Indices de la tabla `device`
--
ALTER TABLE `device`
  ADD PRIMARY KEY (`ID_DEVICE`),
  ADD KEY `DEVICE_FK0` (`ID_LOCATION`),
  ADD KEY `DEVICE_FK1` (`ID_AD`);

--
-- Indices de la tabla `emergency_contact`
--
ALTER TABLE `emergency_contact`
  ADD PRIMARY KEY (`ID_EC`);

--
-- Indices de la tabla `location`
--
ALTER TABLE `location`
  ADD PRIMARY KEY (`ID_LOCATION`),
  ADD KEY `LOCATION_FK0` (`ID_CITY`);

--
-- Indices de la tabla `patient`
--
ALTER TABLE `patient`
  ADD PRIMARY KEY (`ID_PATIENT`);

--
-- Indices de la tabla `patient_condition`
--
ALTER TABLE `patient_condition`
  ADD PRIMARY KEY (`ID_PC`),
  ADD KEY `PATIENT_CONDITION` (`ID_CONDITION`);

--
-- Indices de la tabla `patient_service`
--
ALTER TABLE `patient_service`
  ADD PRIMARY KEY (`ID_PS`),
  ADD KEY `PATIENT_SERVICE_FK5` (`ID_EC`),
  ADD KEY `PATIENT_SERVICE_FK4` (`ID_SPA`),
  ADD KEY `PATIENT_SERVICE_FK3` (`ID_ADMIN`),
  ADD KEY `PATIENT_SERVICE_FK2` (`ID_CAREGIVER`),
  ADD KEY `PATIENT_SERVICE_FK1` (`ID_PATIENT`),
  ADD KEY `PATIENT_SERVICE_FK0` (`ID_DEVICE`);

--
-- Indices de la tabla `province`
--
ALTER TABLE `province`
  ADD PRIMARY KEY (`ID_PROVINCE`),
  ADD KEY `PROVINCE_FK0` (`ID_REGION`);

--
-- Indices de la tabla `region`
--
ALTER TABLE `region`
  ADD PRIMARY KEY (`ID_REGION`);

--
-- Indices de la tabla `resolution`
--
ALTER TABLE `resolution`
  ADD PRIMARY KEY (`ID_RA`),
  ADD KEY `RESOLUTION_FK0` (`ID_SPA`);

--
-- Indices de la tabla `sp_alert`
--
ALTER TABLE `sp_alert`
  ADD PRIMARY KEY (`ID_SPA`),
  ADD KEY `SP_ALERT_FK0` (`ID_ALERT`);

--
-- Indices de la tabla `status`
--
ALTER TABLE `status`
  ADD PRIMARY KEY (`ID_STATUS`);

--
-- Restricciones para tablas volcadas
--

--
-- Filtros para la tabla `admin`
--
ALTER TABLE `admin`
  ADD CONSTRAINT `ID_ADMIN_FK0` FOREIGN KEY (`ID_CITY`) REFERENCES `city` (`ID_CITY`);

--
-- Filtros para la tabla `ambient_data`
--
ALTER TABLE `ambient_data`
  ADD CONSTRAINT `AMBIENT_DATA_FK0` FOREIGN KEY (`ID_STATUS`) REFERENCES `status` (`ID_STATUS`);

--
-- Filtros para la tabla `city`
--
ALTER TABLE `city`
  ADD CONSTRAINT `CITY_FK0` FOREIGN KEY (`ID_PROVINCE`) REFERENCES `province` (`ID_PROVINCE`);

--
-- Filtros para la tabla `device`
--
ALTER TABLE `device`
  ADD CONSTRAINT `DEVICE_FK0` FOREIGN KEY (`ID_LOCATION`) REFERENCES `location` (`ID_LOCATION`),
  ADD CONSTRAINT `DEVICE_FK1` FOREIGN KEY (`ID_AD`) REFERENCES `ambient_data` (`ID_AD`);

--
-- Filtros para la tabla `location`
--
ALTER TABLE `location`
  ADD CONSTRAINT `LOCATION_FK0` FOREIGN KEY (`ID_CITY`) REFERENCES `city` (`ID_CITY`);

--
-- Filtros para la tabla `patient_condition`
--
ALTER TABLE `patient_condition`
  ADD CONSTRAINT `PATIENT_CONDITION` FOREIGN KEY (`ID_CONDITION`) REFERENCES `condition_p` (`ID_CONDITION`);

--
-- Filtros para la tabla `patient_service`
--
ALTER TABLE `patient_service`
  ADD CONSTRAINT `PATIENT_SERVICE_FK0` FOREIGN KEY (`ID_DEVICE`) REFERENCES `device` (`ID_DEVICE`),
  ADD CONSTRAINT `PATIENT_SERVICE_FK1` FOREIGN KEY (`ID_PATIENT`) REFERENCES `patient` (`ID_PATIENT`),
  ADD CONSTRAINT `PATIENT_SERVICE_FK2` FOREIGN KEY (`ID_CAREGIVER`) REFERENCES `caregiver` (`ID_CAREGIVER`),
  ADD CONSTRAINT `PATIENT_SERVICE_FK3` FOREIGN KEY (`ID_ADMIN`) REFERENCES `admin` (`ID_ADMIN`),
  ADD CONSTRAINT `PATIENT_SERVICE_FK4` FOREIGN KEY (`ID_SPA`) REFERENCES `sp_alert` (`ID_SPA`),
  ADD CONSTRAINT `PATIENT_SERVICE_FK5` FOREIGN KEY (`ID_EC`) REFERENCES `emergency_contact` (`ID_EC`);

--
-- Filtros para la tabla `province`
--
ALTER TABLE `province`
  ADD CONSTRAINT `PROVINCE_FK0` FOREIGN KEY (`ID_REGION`) REFERENCES `region` (`ID_REGION`);

--
-- Filtros para la tabla `resolution`
--
ALTER TABLE `resolution`
  ADD CONSTRAINT `RESOLUTION_FK0` FOREIGN KEY (`ID_SPA`) REFERENCES `sp_alert` (`ID_SPA`);

--
-- Filtros para la tabla `sp_alert`
--
ALTER TABLE `sp_alert`
  ADD CONSTRAINT `SP_ALERT_FK0` FOREIGN KEY (`ID_ALERT`) REFERENCES `alert` (`ID_ALERT`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
