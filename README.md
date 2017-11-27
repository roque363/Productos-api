# Productos-api

- Ejecutar los siguientes comandos para crear nuestra base de datos tienda

CREATE SCHEMA IF NOT EXISTS `tienda` DEFAULT CHARACTER SET utf8 ;
USE `tienda` ;

CREATE TABLE IF NOT EXISTS `tienda`.`productos` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `nombre` VARCHAR(100) NOT NULL,
  `precio` DECIMAL(10,2) NOT NULL,
  `imagen` VARCHAR(100) NULL,
  `detalles` VARCHAR(500) NULL,
  `estado` CHAR(1) NOT NULL DEFAULT '1',
  PRIMARY KEY (`id`))
ENGINE = InnoDB;
